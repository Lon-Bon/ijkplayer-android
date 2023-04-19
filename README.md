本项目是基于ijkplayer项目k0.8.8的tag修改而来，整个项目的源码的修改请参考：https://github.com/Lon-Bon/ijkplayer
这个项目是给jitpack看的，依赖于前面生成的so库问题，这里是生成jitpack远程依赖，整个项目只有安卓的部分。

### 如何使用

- 引入jitpack路径：

```groovy
buildscript {
    repositories {
		
        maven { url "https://jitpack.io" }
     
    }
}

allprojects {
    repositories {
        	maven { url "https://jitpack.io" }
        }
    }
}    

```

- 引入项目依赖：

```groovy
	# required, enough for most devices.
    implementation 'com.github.Lon-Bon.ijkplayer-android:ijkplayer-java:0.8.8'
    implementation 'com.github.Lon-Bon.ijkplayer-android:ijkplayer-armv7a:0.8.8'

    # Other ABIs: optional
    implementation 'com.github.Lon-Bon.ijkplayer-android:ijkplayer-armv5:0.8.8'
    implementation 'com.github.Lon-Bon.ijkplayer-android:ijkplayer-arm64:0.8.8'
    implementation 'com.github.Lon-Bon.ijkplayer-android:ijkplayer-x86:0.8.8'
    implementation 'com.github.Lon-Bon.ijkplayer-android:ijkplayer-x86_64:0.8.8'

    # ExoPlayer as IMediaPlayer: optional, experimental
    implementation 'com.github.Lon-Bon.ijkplayer-android:ijkplayer-exo:0.8.8'

//上面需要哪个版本选择依赖哪个
```

