# android_hid
Use Android as Rubber Ducky against targeted Android device or PC

## HID attack using Android

Using Android as Rubber Ducky against Android or Windows. This is not a new technique, just a demo how to perform HID attack using Android instead of rubber ducky. For targeted Android device it is not necessary to be rooted, have ADB/USB debugging enabled and device authorized, since attacker's smartphone behaves as connected keyboard. 

hid_attack - script contains customized commands that are executed (typed) against targeted Android device
hid_pc - script contains customized commands that are executed (typed) against targeted Windows 10

### How to prevent this happening on Android
1) charge you smartphone using you own adapter
2) use none trivial PIN or password lockscreen protection
3) use mobile security software that will detect and prevent from launching payloads

### How to prevent this happening on PC
1) Don't let anyone charge their smartphones in your PC
2) Use security software that will detect Metasploit payload
3) USB condom should help

### PoC
Android: https://youtu.be/aOWr6rWhsIs </br>
PC: https://youtu.be/PJbqZm73MOc

### Prerequisites
- rooted Android with HID kernel support (e.g. NetHunter ROM)
- OTG cable

### Video Tutorial using NetHunter
[![Watch the video](https://i.ibb.co/m0Ng2bc/thumbnail2.png)](https://youtu.be/bYfict-752k)
In the video was used "part1/msf_install" PoC script. Tested payload is removed.

### Video Tutorial without using NetHunter
[![Watch the video](https://i.ibb.co/yYv4gkK/Social-Media-Conference-You-Tube-Thumbnail.png)](https://youtu.be/Mek9DMGy8os)
USB Gadget Tool: https://github.com/tejado/android-usb-gadget </br>
HID gadgets: https://github.com/pelya/android-keyboard-gadget/tree/master/hid-gadget-test </br>
For easy access, I copied USB Gadget Tool and HID gadget to https://github.com/androidmalware/android_hid/tree/main/part2 </br>



### Script info
This is custom script, which might not work on your testing case scenario. Because of that, you must play around with pressed keys that are sent to targeted device. Website with my testing payload is not active anymore. List of all possible keys can be found on the link below.

### Execute command
bash hid_attack
bash hid_pc

### How to flash custom ROM with HID support
https://github.com/pelya/android-keyboard-gadget

### Brute-force pin using Android as HID
https://github.com/urbanadventurer/Android-PIN-Bruteforce

### List of all keys
https://github.com/anbud/DroidDucky/blob/master/droidducky.sh
