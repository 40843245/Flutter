# glance at configurations and code in Flutter project

As a beginner, to know why the screen looks like so and how to make your UI, you just have to concern these files:

+ `lib\main.dart`: a file which display the result on screen when running app you develope on the emulator or real device. It contains an entry point function -- `main` function.

The block in `main` function will be executed once you run the app. You can think `lib\main.dart as `MainActivity.kt` in Android studio when developing an Android App.

+ `pubspec.yaml`: a file that contains configurations about the Flutter project. Including these fields.
  - `name`: the word is self-explanatory, name of your Flutter project.
  - `description`: the word is also self-explanatory, descriptuon of your Flutter project.
  - `version`: the word is also self-explanatory also, currently used version of your Flutter project.
  - `environment`: environment settings, including currently used version of Flutter SDK (written as this format `sdk: ^3.6.0`)
  - `dependencies`: the word is also self-explanatory, all dependencies that will be downloaded and loaded to your Flutter project. When using a class that belongs third-party dependency, please add the dependency in this field.
  - `dev_dependencies`: all dependencies that will be downloaded and loaded to your Flutter project for internal developement and test.
  - `flutter`: configurations to Flutter packages.
 
  etc.
