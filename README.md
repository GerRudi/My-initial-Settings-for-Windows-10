# My-initial-Settings-for-Windows-10
The first things I do and block when reinstalling Windows 10 - mainly as a reminder for myself. 


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


# Group policies

# Registry Settings

# Other cleanup
