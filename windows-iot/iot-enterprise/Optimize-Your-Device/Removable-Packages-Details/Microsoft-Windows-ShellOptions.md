---
title: Package - Shell Accessories
author: twarwick
ms.author: twarwick
ms.date: 1/12/2023
ms.topic: article
ms.prod: windows-iot
ms.technology: iot
description: Removable Package Details for Microsoft-Windows-ShellOptions
keywords: IoT Enterprise, removable packages, storage
---

# Package: Shell Accessories

## Description
Modern Calculator, Character Map, More Icons DLL

**Package Name:** Microsoft-Windows-ShellOptions

**Size:** Approximately 657 KB


## Removing Package

### Online Servicing 
Use the [DISM command-line tool](/windows-hardware/manufacture/desktop/what-is-dism) with the ```/Online``` command-line parameter to remove a single package via online servicing.

```powershell
Dism.exe /Online /LogPath:%WINDIR%\Temp\Microsoft-Windows-ShellOptions.log /NoRestart /Disable-Feature /FeatureName:Microsoft-Windows-ShellOptions /PackageName:@Package
````
### Offline Servicing
Use the [DISM command-line tool](/windows-hardware/manufacture/desktop/what-is-dism) with the ```/Image:<image path>``` command-line parameter to remove a single package via offline servicing.

```powershell
Dism.exe /Image:c:\offline /LogPath:%WINDIR%\Temp\Microsoft-Windows-ShellOptions.log /NoRestart /Disable-Feature /FeatureName:Microsoft-Windows-ShellOptions /PackageName:@Package
````

## File List
| File Name | Installed Location |
|-----------|--------------------|
| character map.lnk | %programdata%\microsoft\windows\start menu\programs\accessories\system tools\character map.lnk |
| bopomofo.uce      | %windir%\system32\bopomofo.uce |
| calc.exe          | %windir%\system32\calc.exe |
| charmap.exe       | %windir%\system32\charmap.exe |
| gb2312.uce        | %windir%\system32\gb2312.uce |
| getuname.dll      | %windir%\system32\getuname.dll |
| ideograf.uce      | %windir%\system32\ideograf.uce |
| kanji_1.uce       | %windir%\system32\kanji_1.uce |
| kanji_2.uce       | %windir%\system32\kanji_2.uce |
| korean.uce        | %windir%\system32\korean.uce |
| moricons.dll      | %windir%\system32\moricons.dll |
| shiftjis.uce      | %windir%\system32\shiftjis.uce |
| subrange.uce      | %windir%\system32\subrange.uce |
| moricons.dll.mun  | %windir%\systemresources\moricons.dll.mun  |

## More Resources
- [Removable Packages](/windows/iot/iot-enterprise/Optimize-Your-Device/Removable-Packages)
- [Reduce Disk Footprint](/windows/iot/iot-enterprise/Optimize-Your-Device/Reduce-Disk-Footprint)
- [Device Optimization Overview](/windows/iot/iot-enterprise/Optimize-Your-Device/Overview)