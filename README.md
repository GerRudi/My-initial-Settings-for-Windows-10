# My-initial-Settings-for-Windows-10
The first things I do and block when reinstalling Windows 10 - mainly intended as a reminder for myself. 

Maybe one day I'll make a file to double click that does all this. 


# Before the Installation
If the device came pre-installed with Windows 10 Home and you want to re-install it with Windows 10 Pro, chances are your Device is activated using a digital license with a key somehow stored in the UEFI firmware by the OEM. 

As a result, Windows will NOT ask you which version you want to install and will simply re-install Win 10 Home. 
To bypass this: 
create a file called pid.txt that contains the following information (where XXX == your Windows 10 Pro key). 

``` 
[PID]
Value=XXXXX-XXXXX-XXXXX-XXXXX-XXXXX
```

Save this file on your Installation media in the "source" folder. 



# Inital Setup
Mute Cortana that is suddenly screaming at you, obviously use an offline account and say no to drugs and tailored ads. 

# Windows Settings

## Explorer Settings

Folder Options -> General: 
- Open File Explorer to: **This PC**
- Untick Show recently / frequently used files / folders...

Folder Options -> General: 
- Untick "Hide extensions for known file types"
- Untick "Show sync provieder notifications"
 -Tick "Use check boxes to select items)
- If required, Tick "Show hidden files" and untick "Hide protected files" thingy.


# Group policies (gpedit.msc)

### Computer Configuration -> Administrative Templates -> Windows Components -> Search

Allow Cortana: Disabled

### Computer Configuration -> Administrative Templates -> Windows Components -> Data Collection and Preview Builds
Allow device name to be sent in Windows diagnostic data: Disabled
Allow Telemetry: Disabled


### Computer Configuration -> Administrative Templates -> System

Display Shutdown Event Tracker: Enabled (Always)

-> Ever accidently clicked restart instead of shutdown or vice versa? Now you have a dialog to select a reason that gives you a chance to re-think. 



### Computer Configuration -> Administrative Templates -> System -> User Profiles

Turn off the advertising ID: Enabled


### Computer Configuration -> Administrative Templates -> Windows Components -> Cloud Content
Do not show Windwos tips: Enabled
Turn off Microsoft consumer experiences: Enabled

-> Fuck off Candy Crush and friends

### User Configuration -> Start Menu and Taskbar**
Do not keep history of recently opened documents: Enabled


# Registry Settings

This setting greys out the option to link your account to a Microsoft account. I hope this also blocks Microsoft doing that by itself when using a MS App with an MS account...
``` 
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\PolicyManager\default\Settings\AllowYourAccount
``` 

**DWORD: value = 0**


# Other settings
**Windows Settings -> Personalization -> Colors**
- Choose your color: Dark
- Transparency effects: Off

**Windows Settings -> Personalization -> Lockscreen**
- Get fun facts, tips, tricks, and more on your locks screen: Off - cause you're not the funny guy
- Remove all apps showing status on the lock screen

**Windows Settings -> Personalization -> Start**
- Show suggestions occasionally in Start:  Off


**Windows Settings -> Personalization -> Taskbar**
- Use small taskbar buttons: On

**Windows Settings -> Privacy -> Diagnostics & feedback**
- Disable whatever's enabled

**Windows Settings -> Privacy -> Activity history**
- Keep enabled if you want, but DISABLE "Send my activity history to Microsoft"


# Essential Software
- 7-Zip
- ImageGlass
- KeePass
- FireFox (Add-ons see that other list)
- Notepad++
- VLC Meida Player
- Maybe a copy of Proccess Explorer and even ffmpeg binaries somewhere




