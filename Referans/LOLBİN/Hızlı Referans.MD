# LOLBIN Hızlı Referans

| Binary | Kullanım | Şüpheli Durum |
|---|---|---|
| mshta.exe | Execute | + URL veya vbscript: argümanı |
| rundll32.exe | Execute | + javascript: veya imzasız DLL |
| regsvr32.exe | Execute | + /i:http + scrobj.dll |
| wmic.exe | Execute | process call create komutu |
| wscript.exe | Execute | //e: flag ile uzantı maskeleme |
| msiexec.exe | Execute / Download | /i http:// veya UNC path |
| certutil.exe | Download | -urlcache -split -f |
| bitsadmin.exe | Download / Persist | + URL + lokal path |
| MpCmdRun.exe | Download | -DownloadFile parametresi |
| powershell.exe | Execute / Download | -enc / IEX / DownloadString |
| msbuild.exe | Execute | Temp'te proje dosyası |
| installutil.exe | Execute | /logfile= /LogToConsole=false /U |
| csc.exe | Execute / Compile | Temp'te .cs → .exe derleme |
| cmstp.exe | Execute / UAC Bypass | + .inf dosyası |
| forfiles.exe | Execute | /c parametresinde cmd veya powershell |
| mavinject.exe | Execute / Inject | /INJECTRUNNING + DLL |
| wuauclt.exe | Execute | /UpdateDeploymentProvider + /RunHandlerComServer |
| mmc.exe | Execute / Lateral | -Embedding argümanı |
| odbcconf.exe | Execute | /a {REGSVR + DLL} |
| ntdsutil.exe | Dump | ifm create |
| diskshadow.exe | Dump | + script dosyası argümanı |
| esentutl.exe | Dump / Copy | /y + ntds.dit veya SAM |
| reg.exe | Persist / Dump | save SAM/SYSTEM/SECURITY |
| schtasks.exe | Persistence | /create + Temp/AppData path |
| sc.exe | Persistence | binPath= Temp veya kullanıcı dizini |
| bitsadmin.exe | Persistence | SetNotifyCmdLine parametresi |
| fodhelper.exe | UAC Bypass | ms-settings registry key yazımı |
| eventvwr.exe | UAC Bypass | mscfile registry key yazımı |
| ComputerDefaults.exe | UAC Bypass | ms-settings registry key yazımı |
| sdclt.exe | UAC Bypass | App Paths\control.exe key yazımı |
| vssadmin.exe | Anti-Forensics | delete shadows /all /quiet |
| bcdedit.exe | Anti-Forensics | recoveryenabled No |
| wbadmin.exe | Anti-Forensics | delete catalog / systemstatebackup |
| fsutil.exe | Anti-Forensics | usn deletejournal |
| cipher.exe | Anti-Forensics | /w: + disk yolu |
| fltMC.exe | Defense Evasion | unload SysmonDrv |
| netsh.exe | Firewall / Proxy | portproxy veya firewall rule ekleme |
| nltest.exe | Discovery | /domain_trusts veya /dclist |
| CertReq.exe | Download / Upload | -Post + dış URL |
| finger.exe | Download | dış IP port 79 bağlantısı |