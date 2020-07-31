# thsconline command line tool

## SYSTEM REQUIREMENTS:
Windows 10 only.
Windows 7 users will need to install Microsoft .NET Framework 4.5

It may work with Powershell Core on newer versions, however this has not been tested and may have unexpected results.

## COMMAND LINE PARAMETERS
--- get - the path to retrieve files from (drop extension, see examples below)

Examples:
  >> GET value of /s/yr12/Maths/trialpapers_extension2  will grab all files associated with this website. In this case it will grab the Maths Ext 2 trial papers.
  >> GET value of /json/5340 will grab all files linked with view number 5340. In this case wil

--- filter - filter out particular files (use w. sol to grab files with solutions)
 
Examples
  >> FILTER value of James Ruse, wil grab all James Ruse papers on a page
  >> FILTER value of 2019, wil grab all 2019 on a page

--- filepath - output folder path.

 Examples
  >> FILEPATH value of C:\Temp will download all files to the C:\Temp folder
