# android_hid
Use Android as Rubber Ducky against another Android device

## HID attack using Android

Using Android as Rubber Ducky against Android. This is not a new technique, just a demo how to perform HID attack using Android instead of rubber ducky. For targeted Android device it is not necessary to be rooted, have ADB/USB debugging enabled and device authorized, since attacker's smartphone behaves as connected keyboard. 

### How to prevent this happening
1) charge you smartphone using you own adapter
2) use none trivial PIN or password lockscreen protection
3) use mobile security software that will detect and prevent from launching payloads

### PoC
https://youtu.be/aOWr6rWhsIs 

### Prerequisites
- rooted Android with HID kernel support (e.g. NetHunter ROM)
- OTG cable

### Script info
This is custom script, which might not work on your testing case scenario. Because of that, you must play around with pressed keys that are sent to targeted device. Website with my testing payload is not active anymore. List of all possible keys can be found on the link below.

### Execute command
bash hid_attack

### How to flash custom ROM with HID support
https://github.com/pelya/android-keyboard-gadget

### Brute-force pin using Android as HID
https://github.com/urbanadventurer/Android-PIN-Bruteforce

### List of all keys
https://github.com/anbud/DroidDucky/blob/master/droidducky.sh
