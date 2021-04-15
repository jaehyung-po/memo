## Flutter Issues



#### Launch Background(Splash) Does not Work After Enable Desktop Support

##### cause

- New files below added during enable desktop support.
```
android/app/src/main/res/drawable-v21/launch_background.xml 
android/app/src/main/res/values-night/styles.xml
```

##### solution  

- Compare above files with
```
android/app/src/main/res/drawable/launch_background.xml 
android/app/src/main/res/values/styles.xml
```

- Add mipmap item you want to use on `android/app/src/main/res/drawable-v21/launch_background.xml`
- optional: Add normal theme if you use that on `android/app/src/main/res/values-night/styles.xml`
