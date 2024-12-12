# run code in Flutter project in Android Studio.
Running code in Flutter project does not make any sense, which may suprise you. It also suprised me a lot and spent me at least 30 minutes to solve it.

Take my project for example,

I create a new Flutter project named `testproject1`. Project hierarchy is shown as following figure.
 
<img width="334" alt="image" src="https://github.com/user-attachments/assets/c68be5e1-4df7-4028-8ab9-f2016402de8d" />

1. I have to open project in Android Studio with location `testproject1` to modify code in `...\lib\main.dart` file, which display the execution result on the emulator or real device at run time.

To do that, select the project highlighted as blue and click `OK` button. Shown as following figure.

<img width="316" alt="image" src="https://github.com/user-attachments/assets/4bfa8c99-0d95-4575-955d-445fa52d66c1" />


2. I want to run it in Emulator for Android device, thus I also have to open project in Android Studio with location `testproject1\android` and then click the run icon to run the code on emulator or real device.

To do that, select the project highlighted as blue and click `OK` button. Shown as following figure.

<img width="319" alt="image" src="https://github.com/user-attachments/assets/e1dc2ab7-a2a2-4288-82f1-32109c7c667e" />

Anyway, you have to open two projects if you use Android Studio to develop an app with Flutter, one to modify the code, while another one is to run your code.
