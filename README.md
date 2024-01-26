# thsconline CLI

## System Requirements:

### Windows
Most versions of Windows are supported, provided Windows Powershell 5.0 or 5.1 is installed which includes Windows 10 & Windows 11.
Note: For Windows 7 or Windows Server 2008 R2, please see the notes on version 1.1.

No support for Windows Server Core versions prior to Windows Server 2016.

**Prerequisites**
* Windows Powershell 5.0 or 5.1 (comes preinstalled on Windows 10 & 11)
* .NET 4.6.1 or newer (.NET 4.7.2 recommended)

### MAC OS or Linux 

**Prerequisites**
* Uncompiled Powershell script copy (please email thsconline@gmail.com to request)
* Powershell 7.2
* .NET 6.0

You will need to download the following NUPKG packages manually extracting the DLL and XML files (/lib/net6.0 folder)

[Anglesharp.dll](https://www.nuget.org/packages/AngleSharp)

[System.Buffers.dll](https://www.nuget.org/packages/System.Buffers)

[System.Runtime.CompilerServices.Unsafe.dll](https://www.nuget.org/packages/System.Runtime.CompilerServices.Unsafe)

[System.Text.Encoding.CodePages.dll](https://www.nuget.org/packages/System.Text.Encoding.CodePages)

## Instructions on how to use

When prompted enter the full path to a page to download files from (minus .html) e.g. to download Year 12 Maths trial papers
type in /s/yr12/Maths/trialpapers_advanced

Then type in your filter (* for all files, or enter a particular year e.g. 2022 or a text search)

Parameters if EXE run by command line. 
- `GET`:  Specify the GET URL
- `FILTER`: Specify the filter (default: all files on a page)
- `FILEPATH`: Specify an alternative file path (default: current folder)

## Feature changes from v1.1 
* Removal of upload functionality which simplifies the functionality.
* Removal of prompt for destination folder. Copy the EXE to the target folder you want the files to be downloaded to.
* Unlike in v1.1 this does not depend on Internet Explorer (MSIE) engine and requires the following DLLs installed to the same folder. A copy suitable for Windows 10 operating system (.NET 4.6.1 or newer) is included but for other Windows or Linux operating system you may need to download the version specific to your .NET version (you can use `nuget`):

[Anglesharp.dll](https://www.nuget.org/packages/AngleSharp)

[System.Buffers.dll](https://www.nuget.org/packages/System.Buffers)

[System.Runtime.CompilerServices.Unsafe.dll](https://www.nuget.org/packages/System.Runtime.CompilerServices.Unsafe)

[System.Text.Encoding.CodePages.dll](https://www.nuget.org/packages/System.Text.Encoding.CodePages)








