# android-quality-starter
setup CheckStyle, FindBugs, PMD and Lint for your Android project easily

This project adds gradle setup for quality tools mentioned above to Android project via shell script. After adding this, we can easily increase quality of the project by static code analysis.

This project is inspired by [vb-android-app-quality](https://github.com/vincentbrison/vb-android-app-quality) application.

Usage
-----

Go to main directory of your Android project and run:

```
curl https://raw.githubusercontent.com/pwittchen/android-quality-starter/master/install.sh | sh
```

Then wait for a while and follow short instruction in the end for quick manual setup.

Remember to add line:

```
apply from: '../config/quality.gradle'
```

to `build.gradle` file of the module you want to check.

Then you can execute the following command in the main directory of the project:

```
./gradlew check
```

Exemplary Android project using this configuration
--------------------------------------------------
- https://github.com/pwittchen/ReactiveNetwork

References
----------
- https://github.com/vincentbrison/vb-android-app-quality
- https://github.com/stephanenicolas/Quality-Tools-for-Android
- http://checkstyle.sourceforge.net/
- http://findbugs.sourceforge.net/
- http://pmd.github.io/
- https://developer.android.com/studio/write/lint.html
