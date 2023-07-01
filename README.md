## ready-project
sample normal codes of a sample projects are here/

---

# XML project
### *build.gradle (: app)*

    implementation 'androidx.core:core-ktx:1.8.0'
    implementation 'androidx.appcompat:appcompat:1.6.1'
    implementation 'com.google.android.material:material:1.9.0'
    implementation 'androidx.constraintlayout:constraintlayout:2.1.4'
    testImplementation 'junit:junit:4.13.2'
    androidTestImplementation 'androidx.test.ext:junit:1.1.5'
    androidTestImplementation 'androidx.test.espresso:espresso-core:3.5.1'

### *build.gradle (Project name)*

    plugins {
        id 'com.android.application' version '8.0.2' apply false
        id 'com.android.library' version '8.0.2' apply false
        id 'org.jetbrains.kotlin.android' version '1.8.20' apply false
    }

---

# Jetpack compose project

### build.gradle (: app)

    implementation 'androidx.core:core-ktx:1.8.0'
    implementation 'androidx.lifecycle:lifecycle-runtime-ktx:2.6.1'
    implementation 'androidx.activity:activity-compose:1.7.1'
    implementation "androidx.compose.ui:ui:$compose_ui_version"
    implementation "androidx.compose.ui:ui-tooling-preview:$compose_ui_version"
    implementation 'androidx.compose.material:material:1.4.2'
    implementation 'com.google.android.gms:play-services-analytics:18.0.2'
    testImplementation 'junit:junit:4.13.2'
    androidTestImplementation 'androidx.test.ext:junit:1.1.5'
    androidTestImplementation 'androidx.test.espresso:espresso-core:3.5.1'
    androidTestImplementation "androidx.compose.ui:ui-test-junit4:$compose_ui_version"
    debugImplementation "androidx.compose.ui:ui-tooling:$compose_ui_version"
    debugImplementation "androidx.compose.ui:ui-test-manifest:$compose_ui_version"

### build.gradle (Project name)

    buildscript{
        ext {
            compose_ui_version = "1.4.0"
        }
    }// Top-level build file where you can add configuration options common to all sub-projects/modules.
    plugins {
        id 'com.android.application' version '7.4.1' apply false
        id 'com.android.library' version '7.4.1' apply false
        id 'org.jetbrains.kotlin.android' version '1.8.0' apply false
    }

---

### Extra dependencies
The useful and helpful dependencies of modes (xml, jetpack compose)

## XML

*[navigation](https://developer.android.com/guide/navigation/get-started#groovy):*
    
    def nav_version = "2.6.0"
    implementation "androidx.navigation:navigation-fragment-ktx:$nav_version"
    implementation "androidx.navigation:navigation-ui-ktx:$nav_version"

*[Retrofit2](https://github.com/square/retrofit):*

    implementation "com.squareup.retrofit2:retrofit:2.9.0"
    implementation "com.squareup.retrofit2:converter-gson:2.9.0"

*[RxJava / RxAndroid](https://github.com/ReactiveX/RxAndroid):*

  *Java:*

    implementation 'io.reactivex.rxjava2:rxjava:2.2.21'
    
  *Android:*    

    implementation 'io.reactivex.rxjava2:rxandroid:2.1.1'
    
  *Adapter:*

    implementation 'com.squareup.retrofit2:adapter-rxjava2:2.9.0'

*Picasso:*

    implementation 'com.squareup.picasso:picasso:2.71828'


## Jetpack compose

*[System Ui Controller:](https://google.github.io/accompanist/systemuicontroller/)*

    implementation 'com.google.accompanist:accompanist-systemuicontroller:0.17.0'

*[navigation compose:](https://developer.android.com/jetpack/compose/navigation)*

    implementation "androidx.navigation:navigation-compose:2.5.3"

*[Live data - state:](https://developer.android.com/jetpack/androidx/releases/compose-runtime)*

    implementation "androidx.compose.runtime:runtime-livedata:$compose_ui_version"

*[Coil:](https://github.com/coil-kt/coil)*

    implementation "io.coil-kt:coil-compose:2.3.0"

*[Coroutines-Android:](https://developer.android.com/kotlin/coroutines)*

    implementation "org.jetbrains.kotlinx:kotlinx-coroutines-android:1.6.1"

*[Lifecycler-viewmodel:](https://developer.android.com/jetpack/androidx/releases/lifecycle)*

    implementation "androidx.lifecycle:lifecycle-viewmodel-ktx:2.6.1"

*[Koin (DI):](https://github.com/burnoo/cokoin)*

    implementation "dev.burnoo:cokoin:1.0.0"
    implementation "dev.burnoo:cokoin-android-viewmodel:1.0.0"
    implementation "dev.burnoo:cokoin-android-navigation:1.0.0"

*[lottie](https://github.com/airbnb/lottie/blob/master/android-compose.md)*

    implementation "com.airbnb.android:lottie-compose:5.2.0"

*[Room:]()*
    
    implementation "androidx.room:room-ktx:2.6.0-alpha01"
    kapt "androidx.room:room-compiler:2.5.1"

  *Don't froget to add `kapt` plugin*
  
  *to add:*
  
  *in `buil.gradle (: app)`*
    
    plugins {
        ...
        id 'kotlin-kapt'
    }


