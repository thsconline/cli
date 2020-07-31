# thsconline command line tool

[Latest Release](https://github.com/thsconline/cmdtool/releases/)

[Download](https://github.com/thsconline/cmdtool/releases/download/v1/thsconline.zip)

## System Requirements:
* Windows 8.1 and Windows 10 supported, with Powershell v4.0 or v5.0 installed.
* Windows 7 will need to install Microsoft .NET Framework 4.5 and Windows Management Framework 4.0.
* Mac and Linux not currently supported. It may work with Powershell Core on newer versions, however this has not been tested and may have unexpected results.

## Comand Line Parameters
* _get_ - the path to retrieve files from (drop extension, see examples below)

Examples:
  > GET value of /s/yr12/Maths/trialpapers_extension2  will grab all files associated with this website. In this case it will grab the Maths Ext 2 trial papers.
  
  > GET value of /json/5340 will grab all files linked with view number 5340. In this case will download all the HSC papers for Maths Ext 2

* _filter_ - filter out particular files (use w. sol to grab files with solutions)
 
Examples
  > FILTER value of James Ruse, wil grab all James Ruse papers on a page
  
  > FILTER value of 2019, wil grab all 2019 papers on a page

* _filepath_ - output folder path.

 Examples
  > FILEPATH value of C:\Temp will download all files to the C:\Temp folder
