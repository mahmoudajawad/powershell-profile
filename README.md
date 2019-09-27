# powershell-profile
My custom PowerShell profile to replicate shell/bash as possible

*CONTINUE AT YOUR OWN RISK: This is a guide meant to share ideas about how to customise your PowerShell expereince. I't s shared here for eductional purposes and not to be used in production environments. It hasn't beed tested thoroughly for any security issues. I take no responsibility for any incident that arise from the use of the methods mentioned in this document.*

Using Windows (10) can be hecic to anyone coming from POSIX-compatible environment. The absence of standard shell/bash isn't something developers can cope with easily. And, although Microsoft worked for years on [PowerShell](https://github.com/PowerShell/PowerShell) implementing good features no body asked for in the console, it still doesn't fee like home for shell/bash users. Hoever, PowerShell comes with good level of customisability that allows users to change key apsects behaviours to make it as much close as possible to shell/bash.

This repo contains a profile file that changes PowerShell behaviours as this:
* Add support for `Ctrl+d` to close the current console.
* Add support fot `tab` to complete the command or file name in shell/bash format rather than rotating over possible values as the default.
* Add support for `Ctrl+l` to clear the current console.
* Adds alias for `findstr` cmdlet as `grep`.
* Adds alias for `vim` as `vi`.

To update your profile to use any of these behaviours simply open [Microsoft.PowerShell_profile.ps1](./Microsoft.PowerShell_profile.ps1) file in this repo and copy the lines which does the behaviour of your choice, or all of them. Then, open PowerShell windows (`Win+x i` is one way to access it). Then type:
```powershell
notepad $PROFILE
```
If no profile is present it would prmopt you to create a new one, click yes. Now paste what you copied earlier in Notepad and save the file. With this your profile is updated you can now enjoy your more like-home expereince in Windows.
