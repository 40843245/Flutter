# project hierarchy in Flutter project (view in Android Studio)
## preface
When you create a new Flutter project in Android Studio, you will see it includes these folders:
+ `.dart_tool`
+ `.idea`
+ `build`
+ `test`
+ `lib`
+ all selected platforms when you create a flutter project.

Here, in this project I selected all platforms -- `Android`,`IOS`,`macOS`,`Linux`,`web` and `Windows`.

So my project hierarchy looks like the following figure.
<img width="334" alt="image" src="https://github.com/user-attachments/assets/b94b34a5-9189-437c-9b15-63ee19c25ac3" />

### What files are stored in these folder respectively? (shown in project hierarchy)
+ `.idea` is a folder that store configurations in Android Studio. It must appear for any kinds of project in Android Studio.

For more details, see [Android studio - should the entire .idea directory be in git ignore?](https://stackoverflow.com/questions/26336709/android-studio-should-the-entire-idea-directory-be-in-git-ignore#:~:text=The%20.idea%20directory%20contains%20a%20set%20of%20configuration,of%20a%20file%2C%20for%20example%2C%20compiler.xml%2C%20encodings.xml%2C%20modules.xml.)

+ `build` is a folder that store files built from a compiler in Android Studio. It must appear for any kinds of project in Android Studio.

+ `test` in Flutter project, is a folder that contains test code for App (by default, it is stored in `widget_test.dart`)

+ `lib` in Flutter project, is a folder that stores `main.dart` file which it is executed when running App. Simply said, the screen of the emulator or real device display the execution result of `main.dart` file.

The other folder is not important for beginners and me. Thus, I will skip it.
