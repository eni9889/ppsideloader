# ++ Tweak Sideloader

This is an Xcode project that will make installing ++ tweaks on a non-jailbroken device super simple. Tested on Xcode 7.3

Supported Apps/Tweaks:
  - YouTube (YouTube ++)
  - Instagram (Instagram ++)
  - Snapchat (Snap + for Snapchat)
  - Facebook (Facebook ++)

How-To:
  - Download Xcode from the Mac app store onto you Mac (https://itunes.apple.com/us/app/xcode/id497799835?mt=12)
  - Connect your computer with your iPhone using your cable
  - Open Xcode
  - Navigate to Xcode -> Preferences -> Accounts
  - Click the + button on the bottom left and sign in with your iTunes username and password
  - Click on the "Personal Team" team and click details
  - Click "Create" next to "iOS Development"
  - Download this project and unzip (https://github.com/eni9889/ppsideloader/archive/master.zip)
  - Inside the new unzipped folder (default called ppsideloader-master) you will find a blank "app.ipa" file. You will need to replace this with a decrypted ipa of the app you are trying to tweak.
  - Find an IPA online of the app you would like to tweak (google something like YouTube IPA download)
  - Once you have downloaded the IPA, rename it so it has the filename "app.ipa"
  - Overwrite the empty "app.ipa" inside the ppsideloader folder with the "app.ipa" file you downloaded earlier.
  - Open "ppsideloader.xcodeproj"
  - Click "ppsideloader" on top left -> Then under targets click "ppsideloader" again
  - Click on the General tab:
  - Change the Bundle Identifier to something unique (i.e james.you.tube)
  - Click on the team dropdown and select "Personal Team"
  - If Xcode complains that there is no provisioning profile click "FIX"
  - ***If you have an App Store version of the app installed on your phone of the app you are trying to tweak you will have to uninstall that version first before the next step!***
  - Click the Play button on the top left and the sideloaded app will start building
  - ***Please note that if this is the first time you are building the app, on your phone go to Settings -> General -> Devices and Trust the new profile***

Known Limitations:
  - ~~YouTube sign in is not currently working~~ FIXED!
  - Snapchat share extension is not currently working

Let me know if this works for you at http://twitter.com/unlimapps

Credits:
  This project was inspired by work that https://twitter.com/dvfying did on https://github.com/Defying/TweakPatcher
