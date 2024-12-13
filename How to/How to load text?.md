# How to load text?
## preface
Here I will discuss how to load string. It does NOT apply for other non-string object.

## From local device
To load string from local device that develops app, follow these steps.

1. Put file that contains the string after serialization under `assets` folder.

2 There are many ways to load that file. The easiest way to load that file is that invoke `rootBundle.loadString` method with asynchronization.
  2.1 To load that file by invoking rootBundle.loadString` method.

   First, import service package with import statements `import 'package:flutter/services.dart' show rootBundle;`

   Next, invoking `rootBundle.loadString` with asynchronization.

   For example,

   To load string from `assets/config.json` file, you can write the following code snippets.
    
   ```
   import 'package:flutter/services.dart' show rootBundle;
    
   Future<String> loadAsset() async {
    return await rootBundle.loadString('assets/config.json');
   }
   ```

## reference
For loading text from assets, see [Loading text assets](https://docs.flutter.dev/ui/assets/assets-and-images#loading-text-assets)
