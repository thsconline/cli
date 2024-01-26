# thsconline CLI

## System Requirements:
* Windows supported, with Windows Powershell v4.0, v5.0 or v5.1 installed.
(Note for Windows 7 and Windows Server 2008 R2, use version 1.1. No support for Windows Server Core versions prior to Windows Server 2016)
* Linux/Mac partially supported but you will need to request the uncompiled Powershell script not EXE by emailing thsconline@gmail.com
and will need to install both .NET 6.0 and Powershell 7.3. This has not been tested.

## Instructions on how to use
This tool may be limited to downloading 40 files at at a time.

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






