## eclipse export MultiProject verification code

- [Japanise-readme.md](readme_ja.md)

- see http://d.hatena.ne.jp/kimukou_26/20130529/p1


- OK1) under ecAbstest
 - ./gradlew clean build


- OK2) under ecAbstest/abstest_ec
  - ./gradlew clean build

- NG) OK2 structure on Android Studio is error

-----------------------------
## Limit of android grade plugin known status

- To see (1 hierarchy or relative path) shallow hierarchy
 - using includeFlat 
 
```
  subprojects{
     version = '1.0'
  }
```

need define (from 0.4.1 run, prepare not need write)

- (The above description does not need If you dive in two-tier project downward as the official site)
 - <= android grade plugin limit?


-----------------------------
## If you do not have the environment path to ANDROID_HOME etc.
 
- gradle.properties Required separately

```
systemProp.android.home='/Applications/android-sdks'
```

Or $HOME/.gradle/gradle.properties put.