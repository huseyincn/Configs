# Starting Android Emulator In Android Studio with parameters
Thanks to stackoverflow (MartinCR and Ivo Stoyanov) created bash script to run with kvm parameters and vulkan option, some mac users use it for no audio option to prevent macOs audio failure with android emulator. However I use this script use kvm in android studio.

```
Android Studio by default uses the binary $ANDROID_SDK/emulator/emulator. In my case the path in MacOS is /Users/martin/Library/Android/sdk/emulator/emulator. What I did is:
Rename the binary to emulator-original

Create a bash script with the name emulator that contains:

/Users/<YOUR_USERNAME>/Library/Android/sdk/emulator/emulator-original <PARAMS> $@```

Change the script permissions with chmod +x emulator
```

I gave the script that i use in my computer at the root level of repository.
