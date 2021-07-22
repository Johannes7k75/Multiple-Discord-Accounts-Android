# Multiple-Discord-Accounts-Android

### Disclaimer
This is a method where you use multiple discord apps. For every Account you want you have to create a new app

### Heres How
1. Download [APK Easy Tool](https://forum.xda-developers.com/t/tool-windows-apk-easy-tool-v1-59-2-2021-04-03.3333960/)
2. Download a Discord Apk. I include one but if you want to make sure you dont get a virus you can download one on yourself or create a.

3. open APK Easy Tool select Browse, navigate to the discord apk and select they  
5. Press on Decompile
6. navigate to the decompiled APK directory. You can get to there with Pressing the Button on the Right.
7. In the Folder you see another Folder with the name of the apk go in there and edit the AndroidManifest.xml
    * Relace the content with the content from the AndroidManifest.xml from this repo
    * Replace the the content <replace with a new package name> with a new package name like discord1, discord2 or something else. **Important it has to be an that dont exist on your phone**   
8. After that on thing navigate to res > values > strings.xml   
  go into line 2090 / where it shows `<string name="discord">Discord</string>`
    * and rename Discord to something other. This is that you can differentiate between the Discord Apps. I renamed then after my Discord Name.
8. Go back into APK Easy Tool and press Compile
9. After it finished press Sign APK
  
10. Then you can install the APK there are two way:  
* copy the APK from your PC to your phone and install it  
    * you can find the APK in the Compiled APK directory  
  
* Use ADB to install the APK  
    * for that you have to be [**A**ndroid **D**ebug **B**ridge](https://developer.android.com/studio/releases/platform-tools) installed
    * the connect you phone to the pc and enable in the Developer Options on your phone USB-Debbuging
    * after you made sure to have that all press install APK it should take some time

A new App should appear on your phone.  
Here you have a second Discord App on your Phone
