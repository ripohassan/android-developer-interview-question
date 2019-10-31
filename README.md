# android-developer-interview-question

Describe android build process.

AAPT Tool
AAPT stands for android assets packaging tool. This tool comes with the Android SDK and present in $ANDROID_HOME/platform-tools/. It takes all the resources present in the res/ directory and compiles them. It generates a R.java file which contains ids of all the resources. Once you have installed the Android SDK you can directly execute the aapt commands.
* Android Build Process Steps
AAPT takes all the resources present in res/ directory and AndroidManifest.xml(meta data of android app) and compiles all the resources. It creates a R.java class which has all the resource ids.

* Then all the java files including R.java gets compiled into byte code.
* Android application runs on dalvik vm so the byte code is cross compiled to the Dalvik byte code (.dex file)
* The .dex file and the compiled resources together forms the .apk file.
* Generated apk file is a debug build, to make a release build we need to sign the apk file using a key. You can do this from Android Studio.
* Once you sign the apk file it will be ready to use in production.
