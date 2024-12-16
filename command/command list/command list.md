# Flutter
## command list
### flutter --version
See current version of Flutter.

#### syntax 
```
flutter --version
```

### flutter --help
See help of all commands or specific command in Flutter command-line tool.

#### syntax 
```
flutter --help ([<flags>]|[<command>])
```

where 

`<command>` are one of command in Flutter command-line tool.

For available `<flags>` and <command>`, see `flutter --help`.

#### examples
##### example1
See help of all commands in Flutter command-line tool.

```
flutter --help
```

##### example2
See help of `create` command in Flutter command-line tool.

```
flutter --help create
```

##### example2
See help of `create` command with verbose in Flutter command-line tool.

```
flutter --help --verbose
```

or 

```
flutter --help -v
```

### flutter create 
List a project with Flutter.

#### syntax 
```
flutter create <your_project_name>
```

restriction of `<your_project_name>`:

`<your_project_name>` MUST satisfy all following rules.

- start with lowercase alphabet letter
- only consist of lowercase alphabet letter, digit and underscore (`_`)

More details stated in [`quickguide.md#create a new flutter project`](https://github.com/40843245/Flutter/blob/main/quickstart%20guide.md#create-a-new-flutter-project)

More details also stated in `flutter --help create`

### flutter build
Build an executable app or install bundle.

#### syntax 
```
flutter build [<flags> | [<subcommand>] ]
```

More details stated in `flutter --help build`

### flutter pub get
Get public flutter packages that is listed in `dependencies` section under `pubspec.yaml` file.

#### syntax 
```
flutter pub get
```

More details stated in [`flutter: The Flutter command-line tool`](https://docs.flutter.dev/reference/flutter-cli)

More details also stated in `flutter --help pub get`

### flutter pub outdated
Identify outdated public package of Flutter.

#### syntax
```
flutter pub outdated
```

More details stated in [`flutter: The Flutter command-line tool`](https://docs.flutter.dev/reference/flutter-cli)

More details also stated in `flutter --help pub outdated`

### flutter pub upgrade
Upgrade public package of Flutter.

#### syntax
```
flutter pub upgrade
```

More details stated in [`flutter: The Flutter command-line tool`](https://docs.flutter.dev/reference/flutter-cli)

More details also stated in `flutter --help pub upgrade`

### flutter devices
List all available devices that can be developed with Flutter.

#### syntax 
```
flutter devices
```

More details stated in `flutter --help devices`

### flutter emulators
List all available emulators that can be developed with Flutter.

#### syntax 
```
flutter emulators
```

More details also stated in `flutter --help emulators`
