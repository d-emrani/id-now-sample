This sample app showcases the problems when including the id-now sdk to an app.

The following errors are shown during the build:
```
> Task :app:mergeDebugNativeLibs
2 files found for path 'lib/arm64-v8a/libRSSupport.so'. This version of the Android Gradle Plugin chooses the file from the app or dynamic-feature module, but this can cause unexpected behavior or errors at runtime. Future versions of the Android Gradle Plugin may throw an error in this case.
Inputs:
 - /Users/emrani/Library/Android/sdk/build-tools/30.0.3/renderscript/lib/packaged/arm64-v8a/libRSSupport.so
 - /Users/emrani/.gradle/caches/transforms-3/f31420f5d01a727cfce83d37140720c7/transformed/idnow-platform-4.19.1/jni/arm64-v8a/libRSSupport.so

2 files found for path 'lib/arm64-v8a/librsjni_androidx.so'. This version of the Android Gradle Plugin chooses the file from the app or dynamic-feature module, but this can cause unexpected behavior or errors at runtime. Future versions of the Android Gradle Plugin may throw an error in this case.
Inputs:
 - /Users/emrani/Library/Android/sdk/build-tools/30.0.3/renderscript/lib/packaged/arm64-v8a/librsjni_androidx.so
 - /Users/emrani/.gradle/caches/transforms-3/f31420f5d01a727cfce83d37140720c7/transformed/idnow-platform-4.19.1/jni/arm64-v8a/librsjni_androidx.so

2 files found for path 'lib/armeabi-v7a/librsjni_androidx.so'. This version of the Android Gradle Plugin chooses the file from the app or dynamic-feature module, but this can cause unexpected behavior or errors at runtime. Future versions of the Android Gradle Plugin may throw an error in this case.
Inputs:
 - /Users/emrani/Library/Android/sdk/build-tools/30.0.3/renderscript/lib/packaged/armeabi-v7a/librsjni_androidx.so
 - /Users/emrani/.gradle/caches/transforms-3/f31420f5d01a727cfce83d37140720c7/transformed/idnow-platform-4.19.1/jni/armeabi-v7a/librsjni_androidx.so

2 files found for path 'lib/x86/libRSSupport.so'. This version of the Android Gradle Plugin chooses the file from the app or dynamic-feature module, but this can cause unexpected behavior or errors at runtime. Future versions of the Android Gradle Plugin may throw an error in this case.
Inputs:
 - /Users/emrani/Library/Android/sdk/build-tools/30.0.3/renderscript/lib/packaged/x86/libRSSupport.so
 - /Users/emrani/.gradle/caches/transforms-3/f31420f5d01a727cfce83d37140720c7/transformed/idnow-platform-4.19.1/jni/x86/libRSSupport.so

2 files found for path 'lib/x86/librsjni_androidx.so'. This version of the Android Gradle Plugin chooses the file from the app or dynamic-feature module, but this can cause unexpected behavior or errors at runtime. Future versions of the Android Gradle Plugin may throw an error in this case.
Inputs:
 - /Users/emrani/Library/Android/sdk/build-tools/30.0.3/renderscript/lib/packaged/x86/librsjni_androidx.so
 - /Users/emrani/.gradle/caches/transforms-3/f31420f5d01a727cfce83d37140720c7/transformed/idnow-platform-4.19.1/jni/x86/librsjni_androidx.so

2 files found for path 'lib/x86_64/libRSSupport.so'. This version of the Android Gradle Plugin chooses the file from the app or dynamic-feature module, but this can cause unexpected behavior or errors at runtime. Future versions of the Android Gradle Plugin may throw an error in this case.
Inputs:
 - /Users/emrani/Library/Android/sdk/build-tools/30.0.3/renderscript/lib/packaged/x86_64/libRSSupport.so
 - /Users/emrani/.gradle/caches/transforms-3/f31420f5d01a727cfce83d37140720c7/transformed/idnow-platform-4.19.1/jni/x86_64/libRSSupport.so

2 files found for path 'lib/x86_64/librsjni_androidx.so'. This version of the Android Gradle Plugin chooses the file from the app or dynamic-feature module, but this can cause unexpected behavior or errors at runtime. Future versions of the Android Gradle Plugin may throw an error in this case.
Inputs:
 - /Users/emrani/Library/Android/sdk/build-tools/30.0.3/renderscript/lib/packaged/x86_64/librsjni_androidx.so
 - /Users/emrani/.gradle/caches/transforms-3/f31420f5d01a727cfce83d37140720c7/transformed/idnow-platform-4.19.1/jni/x86_64/librsjni_androidx.so


> Task :app:stripDebugDebugSymbols
Unable to strip the following libraries, packaging them as they are: libPhoenixAndroid.so, libRSSupport.so, libZoomDummy.so, libidnow_tracking.so, libimage_processing_util_jni.so, librsjni.so, librsjni_androidx.so.
```
