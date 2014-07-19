/*
Title: logcat
Sort: 1
*/

All should be done from cmd

`adb logcat CordovaLog:D *:S`
`adb logcat AndroidRuntime:E dalvikvm:S GCM:D memtrack:S android.os.Debug:S eglCodecCommon:S jdwp:S linker:E SoundPool:S AudioService:S IInputConnectionWrapper:E WindowManager:E`

Connect to device
------------------
`adb -s 7f1c864e ....`

`adb -d logcat ...`



console.log from device
`adb -d logcat chromium:I *:S`

Target Device
-d Direct an adb command to the only attached USB device.
-e Direct an adb command to the only running emulator instance.
