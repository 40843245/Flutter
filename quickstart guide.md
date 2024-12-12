# Flutter
## quickstart guide
### install Flutter SDK
To install Flutter SDK,

1. open `Git Bash` terminal.
2. Type following command

```
git clone -b stable https://github.com/flutter/flutter.git
```

3. Find location of flutter SDK, the default location may be `C:\...\flutter\bin`, you should see there is a `dart.exe`. Then, set the location to system environment variable `PATH`.

For more details, stated in [【Flutter基礎概念與實作】 Day1–Flutter是什麼，能吃嗎?](https://ithelp.ithome.com.tw/articles/10215158) 

### create a new flutter project
There are two ways: one is through command on command prompt, another one is through Android Studio IDE.

#### 1st way
To open create a new flutter project, following these steps:

1. Open command prompt.
2. Type following command

```
flutter create <your_project_name>
```

restriction of `<your_project_name>`:

<your_project_name> MUST satisfy all following rules.

+ start with lowercase alphabet letter
+ only consist of lowercase alphabet letter, digit and underscore (`_`)

##### examples of project name
Examples of **valid** project name include

+ `testproject1`

Examples of **invalid** project name include

+ `testProject1` (it contains uppercase alphabet letter, which violates second rule)
+ `_testproject1` (it does NOT start with lowercase alphabet letter, which violate first rule)

#### 2nd way
To open create a new flutter project, following these steps:

1. Open Android Studio IDE.
2. Install `Flutter` plugin from Androidn Studio marketplace (if not installed yet) and enable it (if not enabled yet).
3. Click create new flutter project.
4. Select `Flutter` option, specify the location of `Flutter SDK` to `Flutter SDK path`, click `Next` Button.

<img width="598" alt="image" src="https://github.com/user-attachments/assets/690661af-5887-4a5b-9e0a-e1fa96ec31a8" />

5. Type your project name, also check other configurations.

<img width="587" alt="image" src="https://github.com/user-attachments/assets/9b148ae8-fa9c-4850-8dfc-ad57752b9356" />

6. Click `Create` Button. 

