This sample app showcases the problems when including the id-now sdk to an app.

⚠️ **Make sure NDK version 23.2.8568313 is installed (via Android Studio SDK manager)**

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
/Users/emrani/Library/Android/sdk/ndk/23.2.8568313/toolchains/llvm/prebuilt/darwin-x86_64/bin/llvm-strip: error: program header with offset 0x23ef80 and file size 0xb080 goes past the end of the file

/Users/emrani/Library/Android/sdk/ndk/23.2.8568313/toolchains/llvm/prebuilt/darwin-x86_64/bin/llvm-strip: error: Info field value 22 in section .rela.plt is invalid

/Users/emrani/Library/Android/sdk/ndk/23.2.8568313/toolchains/llvm/prebuilt/darwin-x86_64/bin/llvm-strip: error: '/Users/emrani/AndroidStudioProjects/IdNowSample/app/build/intermediates/merged_native_libs/debug/out/lib/x86_64/libPhoenixAndroid.so': The file was not recognized as a valid object file

/Users/emrani/Library/Android/sdk/ndk/23.2.8568313/toolchains/llvm/prebuilt/darwin-x86_64/bin/llvm-strip: error: '/Users/emrani/AndroidStudioProjects/IdNowSample/app/build/intermediates/merged_native_libs/debug/out/lib/x86/libZoomDummy.so': The file was not recognized as a valid object file

Unable to strip the following libraries, packaging them as they are: libPhoenixAndroid.so, libZoomDummy.so.
```
