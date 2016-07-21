# ++ Tweak Sideloader

This is an Xcode project that will make installing ++ tweaks on a non-jailbroken device super simple. Tested on Xcode 7.3

***Please note that in iOS 10 push notifications no longer work for some people :(. Follow these directions for a workaround: http://www.twitlonger.com/show/n_1soqbs5 OR https://www.youtube.com/watch?v=HuurPfvaros***

***Please note that now apple expires certificates in 7 days for free developer account*** - https://www.reddit.com/r/jailbreak/comments/4hotx3/news_free_developer_account_installs_reduced_to_7/

Supported Apps/Tweaks: 
  - Poke Go ++ for Pokemon Go (MAKE SURE TO SET KEEP_ORIGINAL_APP_NAME TO `YES` FOR THIS TWEAK)
  - YouTube (YouTube ++)
  - Instagram (Instagram ++)
  - Snapchat (Snap + for Snapchat)
  - Facebook (Facebook ++)
  - WhatsApp ++
  - Twitter ++
  - Vine ++

Descriptions at http://beta.unlimapps.com/

***How-To Video:*** https://youtu.be/SmV4A_p7WWY

***For Help Visit:*** https://www.reddit.com/r/sideloaded

How-To:
  - Download Xcode from the Mac app store onto you Mac (https://itunes.apple.com/us/app/xcode/id497799835?mt=12)
    (If you have iOS 10 you will need Xcode 8 beta, unfortunately cannot give link here, legal reasons)
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

Configuration (modify values in PP_SIDELOADER_OPTIONS):
  - ***KEEP_ORIGINAL_APP_NAME:*** Do not add ++ to the installed app name
  - ***OVERWRITE_ORIGINAL_APP:*** If you want push notifications keep this true. If you want to install a duplicate app without push notifications set this to false
  - ***CREATE_IPA_FILES:*** If you set this to true after every build you will see an IPA with ++ in the products directory inside your project folder.

Let me know if this works for you at http://twitter.com/unlimapps

Credits:
  This project was inspired by work that https://twitter.com/dvfying did on https://github.com/Defying/TweakPatcher
