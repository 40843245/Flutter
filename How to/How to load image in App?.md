# How to load image in App?
## For local device
To load a local device that develops app, follow these steps.

1. Put your image under `assets` folder.
 
2. Specify your image in assets field in `pubspec.yaml`. 

3. Load image with `Image.assets` static method.

### example

For example,

To use `my_icon.png`,

1. Put `my_icon.png` in `...\assets\my_icon.png`, then in `pubspec.yaml`, specify `my_icon.png` in `pubspec.yaml`. 

Looks like this:

In `pubspec.yaml`. 

```
flutter:
  assets:
    - assets/my_icon.png
```

> [!NOTE]
> NOTICE that in YAML,
>
> A subfield in a field must indent two spaces more than the field has,
>
> thus `assets` field must be indented two spaces.
> 
> Otherwise, you will see an error -- `Error: unable to find directory entry in pubspec.yaml`.

2. Load image with `Image.assets` static method.

```
//...
Image.assets(
  `my_icon.png`
  // other arguments
)
//...
```

## reference

For how to add images to assets, see [Adding assets and images](https://docs.flutter.dev/ui/assets/assets-and-images)

For how to load images, see [How to add image in Flutter? (stackoverflow)](https://stackoverflow.com/questions/50903106/how-to-add-image-in-flutter)
