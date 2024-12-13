# How to load image in App?
## For local device
To load a local device that develops app, follow these steps.

1. Declare your image in assets field in `pubspec.yaml`.

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
