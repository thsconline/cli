# thsconline CLI

## System Requirements:
* Windows 8.1 and Windows 10 supported, with Powershell v4.0 or v5.0 installed.
* Windows 7 will need to install Microsoft .NET Framework 4.5 and Windows Management Framework 4.0.
* Mac and Linux not currently supported. It may work with Powershell Core on newer versions, however this has not been tested and may have unexpected results.

## User Requirements
* Requires a BoredofStudies account to be able to use.

## Initial Setup
When first opening the application, it will ask you to authenticate, ask for a default download folder, then you can select a library and a folder to view.

## Available Libraries
* _bos_ (or _boredofstudies_)- Bored of Studies resources section.
* _drive_ & _fz_ - Google Drive. 
* _nanahcub_ - Maths exam papers
* _nesa_ (or _bostes_, _hsc_, _hscexams_, _hscpapers_) - HSC exam papers (NESA website)
* _thsc_ (or _s_, _files_, _thsconline_) - thsconline website 
* _web_ - Any other webpage

## Command Line Parameters
* _BACK_ - Navigate to the last viewed folder.


* _CLEAR_ - Clear console
* _DOWNLOAD_ - Download file. Some libraries will prompt for a filename, as download mechanism differs for some libraries.
    * _thsc_ - For this library, for almost all pages, enter a filter value as the parameter rather, as the links are not numbered for some pages. This uses the multiple file downloader implemented in v1.1.
    * Files with non-English characters are not currently supported. Please use the Custom option.
    
* _EXIT_ or _QUIT_ - Exit program.
* _GET_ - Navigate to link or file. Links are numbered. The GET command can also be used to download files in some libraries
    * _bos_ - For this library, this command is the same as the _GOTO_ command.
* _GET PAGE_ or _VIEW PAGE_ - (for _bos_ library only) Change page.
    
* _GOTO_ - Navigate to different folder:
    * _bos_ - Use the collection name (no link numbering). To view all the collections use the command _GET /resources_.
    * _drive_ - Use the command _CHANGE LIBRARY_ to enter a new Google Drive folder ID.
    * _fz_ - Enter link number or the unique folder identifier (this is different to the Google Drive ID)
    * _nanahcub_ & _web_ - Enter link number or a URL
    * _nesa_ - Enter year or year followed by the exam pack. (The part of the URL after https://educationstandards.nsw.edu.au/wps/portal/nesa/resource-finder/hsc-exam-papers/)
    * _thsc_ - Enter link number or relative path. (The part of the URL after https://thsconline.github.io/, unlike v1.1 retain the extension, although the /files/ folder can be dropped from the path e.g. _GOTO /s/yr12/Maths/trialpapers.html_). Some pages do not have link numbering for some links.
    * **Note:** The _GOTO_ command cannot be used to download files.
* _HELP_ or _GET HELP_ - Show basic help information
* _OPEN_ - This command is the same as the _DOWNLOAD_ command for some libraries, except it will attempt to open the file.


* _REFRESH_ or _RELOAD_ - Clear console
* _RESET_ - Return to default folder. 

* _SET FOLDER_ - Change default download folder
* _SET LIBRARY_ or _CHANGE LIBRARY_ - Change library and default folder

* _VIEW PROPERTIES_ or _QUERY_PROPERTIES_ - Show current library and default download folder 
* _VIEW USER_ or _QUERY USER_ - Show current logged in user. To change which user is logged in requires restarting the application.
* _VIEW WEBSITE_ or _VIEW_ - Show HTML of current page in new window. 
    * _nanahcub_ & _web_ - This will open the page in default browser rather than in a small popup window as for other
    * _thsc_ - Enter filter value to open viewer of file (if multiple results are returned, it will prompt for a selection). Entering no value will revert to default behaviour of opening the page as per the _VIEW WEBSITE_ command.
