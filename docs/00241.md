# 扫描转台将物体数字化为 3D 模型

> 原文：<https://hackaday.com/2012/04/27/scanning-turntable-digitizes-objects-as-3d-models/>

这个转盘[可以自动数字化物体，以便在类似 Blender3D 的 3D 渲染软件](http://www.youtube.com/watch?v=BF7QUtghGi8)中使用。[詹姆斯·达尔比]用高质量的 DSLR 和他的垃圾箱里的一些零碎东西建造了它。转盘本身就是一个翻转过来的懒苏珊。旋转模型的底座通常是放在桌子上的东西，但这种方式给他一个放置模型的区域，较大的部分作为驱动机构的安装面。

他使用扫描仪的步进电机，以及打印机的皮带和张力硬件来驱动平台。这是由连接到 Arduino 的晶体管阵列(ULN2003 芯片)驱动的。微控制器还控制相机的快门。休息之后我们加入了他的代码。你会发现他的演示视频也嵌入其中。

这个概念与我们见过的其他转盘构建相同，但是詹姆斯将后期处理更进了一步。他不是仅仅制作一个旋转的 gif，而是使用 [Autodesk 123D](http://www.123dapp.com/) 从这组图像中创建一个数字模型。

[https://www.youtube.com/embed/BF7QUtghGi8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/BF7QUtghGi8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

```
int camera = 13;
int startButton = 3;

long stepCount = 0;
long stepErrorCount = 0;
int callibrated = LOW;
int photos = 10;
int turns = 0;

int buttonPrep = 0;

unsigned long actualStepsPerRevolution = 1; //keep this at 1 or it gets confused somewhere.

unsigned long serialMode = 0; //to store serial data pulled from void getSerial()
int inbyte;

#include &lt;Stepper.h&gt;
int stepsPerRevolution = 13546; //13546 is about right if you can't be bothered to callibrate.
Stepper myStepper(stepsPerRevolution, 6,8,7,9);

void setup() {
  pinMode(camera, OUTPUT);

  myStepper.setSpeed(1); // set the speed in rpm based on stepsPerRevolution

  Serial.begin(9600);
  Serial.println(&quot;DalbySpin9002, contact@jamesdalby.co.uk&quot;);
  Serial.println();
  Serial.println(&quot;Photos required? (eg, '36/')&quot;);

  serialMode = 0;
  while (serialMode == 0) getSerial();
  Serial.println();
  photos = serialMode;
  Serial.print(photos);
  Serial.println(&quot; photos to take.&quot;);

  if(photos &gt; 360){///////////////////////warn if asked to take too many photos
  Serial.println(&quot;Hmm, taking this many photos probably wont go to well but you're probably going to try anyway so good luck with that!&quot;);
  delay(2000);}

  Serial.println();
  Serial.print(&quot; Positioning for Calibration...&quot;);
}

void loop() {

//CALLIBRATION
 while (turns &lt; 2){
   while (digitalRead(startButton) == LOW &amp;&amp; turns &lt; 2){
    stepAdv(1,0);//go one step
   }

   if (digitalRead(startButton) == HIGH){
     while (digitalRead(startButton) == HIGH) stepAdv(1,0);//go one step
     turns = turns + 1;
     if (turns == 1){ Serial.println(&quot; Done.&quot;);
     Serial.print(&quot; Calibrating...&quot;);}

     if (turns == 2){
       stepsPerRevolution = stepCount;//  divide one rotation up into a series of photos

       Serial.println(&quot; Done.&quot;);
       Serial.print(&quot; Recorded steps for one revolution = &quot;); Serial.println(stepCount);
     }
     stepCount = 0;
     delay(5000);
   }
 }
//END OF CALLIBRATION

//GO CODE:

 if (turns &gt;= 2 ){
   Serial.println();
  Serial.println(&quot;Capturing:&quot;);
  delay(9999);

  int photoCount = 1;
  for (int i=1; i &lt;= photos; i++){

    Serial.print(&quot; Photo &quot;); ///&quot;Photo x of y&quot;
    Serial.print(photoCount);
    Serial.print(&quot; of &quot;);
    Serial.print(photos);

    /*Serial.print(&quot; Steps = &quot;);
    Serial.print(stepCount);*/

    delay(2000);
    digitalWrite(camera, HIGH);  //trigger SLR
    Serial.println(&quot;   CLICK!&quot;);

    delay(2000);
    digitalWrite(camera, LOW);
    photoCount = photoCount + 1;

    stepAdv(stepsPerRevolution/photos, 0); //divide one rotation up into a series of photos
  }
    delay(10);
    while(photoCount &gt;= photos){}

  }

  ///////////////////////////END

 }

void stepAdv(int steps, int mode){
  go(steps);
  stepCheck();

}

void go(int steps1){
  for (int i=1; i &lt;= steps1; i++){
    myStepper.step(1);
    stepCount = stepCount + 1;
   stepCheck();

  }

}

void stepCheck(){

  if (digitalRead(startButton) == HIGH ){
    actualStepsPerRevolution = 0;
   }
  if (digitalRead(startButton) == LOW &amp;&amp; actualStepsPerRevolution == 0){
    actualStepsPerRevolution = stepCount;
  }

 }

long getSerial() ///to set number of photos
{
  serialMode = 0;
  while (inbyte != '/')
  {
    inbyte = Serial.read();
    if (inbyte &gt; 0 &amp;&amp; inbyte != '/')
    {
      serialMode = serialMode * 10 + inbyte - '0';

    }
  }
  inbyte = 0;
  return serialMode;

}
```