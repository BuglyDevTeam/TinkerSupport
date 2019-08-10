# TinkerSupport


解压repo.rar，将repo文件夹放到工程根目录，然后在工程根目录的build.gradle添加

 maven { url uri('./repo') }
```xml
buildscript {
    repositories {
        //这里添加本地依赖
        maven { url uri('./repo') }
        jcenter()
        google()
    }
    dependencies {
        //声明需要依赖的版本
        classpath "com.tencent.bugly:tinker-support:1.1.6"
    }
}
allprojects {
    repositories {
        //这里添加本地依赖
        maven { url uri('./repo') }
        jcenter()
        google()
    }
}
```
 



