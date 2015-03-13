Library StackBlur 
=================

original by https://github.com/kikoso/android-stackblur


usage;

1. clone
2. add to your settings.gladdle
```
include ':StackBlur'
project(':StackBlur').projectDir = new File(settingsDir, '<path-to-clone>')

```
3. add to your dependencies on build.gradle
```
compile project(':StackBlur')

```

4. enjoy
```JAVA
int radio = 5;
BitmapFactory mImage = BitmapFactory.decodeResource(getResources(), R.drawable.myImage);
StackBlurManager stackBlurManager = new StackBlurManager(mImage);
stackBlurManager.process(radio);
mImaveView.setImageBitmap(stackBlurManager.returnBlurredImage());
```





