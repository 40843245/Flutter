# glance at configurations and code in Flutter project
## overview

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

> [!NOTE]
> Very importance notice that you have to take it in mind.
>
> **Neither** edit and modify file except for `lib\main.dart`, **nor** , and create new file, **nor** change the file name, if not neccessary (especially you **DON'T** know what it does).
> 
> Otherwise, you may accidentally encounter an error and thus it may take you for a long time to solve it. 
 
> [!NOTE]
> Very importance notice that you have to take it in mind.
>
> In `lib\main.dart`, it MUST contain exactly one entry point -- `main` function. Otherwise, you will get a compiler error or runtime error.
>
> Also it must invoke `runApp` function in the only one entry point. The code SHOULD look like this:

```
void main() {
  runApp(MyApp());
}
```

or use shorthand syntax for function if one can, as follows.

```
void main() => runApp(MyApp());
```

## details about code in `main.dart`
As stated before, when the app you develop starts runs, the only one entry point -- `main` function will be executed.

Assume that the `main` function is declared as follows.

```
// import statements

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Hello Flutter',
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: MyHomePage(title: 'Flutter Demo Home Page'),
      debugShowCheckedModeBanner: false,
    );
  }
}

//...
```

It will first invoke MyApp class, instantiate a MyApp instance. 

When instantiating MyApp instance, it will invoke overridden `build` method which is annotated by `@override` annotation.

During invoking the overridden `build` method, of course, it will invoke MaterialApp, instantiate a MaterialApp instance and return the instance.

Finally, the `runApp` function will run the MaterialApp instance returned by `build` method and according to this to display it on the screen of emulator or real device.
