This sample app showcases the following bug in the id-now sdk


Adding these two libraries to an app:  

`de.idnow.android.sdk:idnow-platform:4.19.1`

`androidx.appcompat:appcompat:1.5.1`

Will result in this error:

`Duplicate class androidx.lifecycle.ViewModelLazy found in modules lifecycle-viewmodel-2.5.1-runtime (androidx.lifecycle:lifecycle-viewmodel:2.5.1) and lifecycle-viewmodel-ktx-2.3.1-runtime (androidx.lifecycle:lifecycle-viewmodel-ktx:2.3.1)`

`Duplicate class androidx.lifecycle.ViewTreeViewModelKt found in modules lifecycle-viewmodel-2.5.1-runtime (androidx.lifecycle:lifecycle-viewmodel:2.5.1) and lifecycle-viewmodel-ktx-2.3.1-runtime (androidx.lifecycle:lifecycle-viewmodel-ktx:2.3.1)`
