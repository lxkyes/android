# Android Demo By ttdevs

``` java
    signingConfigs {
        release {
            keyAlias 'ttdevs'
            keyPassword 'ttdevs'
            storeFile file('../android.jks')
            storePassword 'ttdevs'
        }
    }

    buildTypes {

        release {
            minifyEnabled false
            proguardFiles getDefaultProguardFile('proguard-android.txt'), 'proguard-rules.pro'
            signingConfig signingConfigs.release
            debuggable true
            jniDebuggable false
            renderscriptDebuggable false
            zipAlignEnabled true
        }
    }
```
