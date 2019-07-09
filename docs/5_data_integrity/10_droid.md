---
layout: default
title: DROID Reporting
nav_order: 10
parent: Data Integrity

---

**_Workflow Type:_ Technical.** This document describes how to create reports using DROID to validate formats and track original file data. 

# DROID


## Uses



1. Create a list of digital file titles that can be saved as a Excel doc or uploaded to Google Drive and linked from a finding aid.
    *   Here’s an example from BPATS (I _think_ this was created using DROID, but not positive): [https://docs.google.com/spreadsheets/d/1o7Kf8V5TnU4HTU0FpnE5vQ5EpbnHbuQdgoH0IfDhv7s/edit#gid=1454817404](https://docs.google.com/spreadsheets/d/1o7Kf8V5TnU4HTU0FpnE5vQ5EpbnHbuQdgoH0IfDhv7s/edit#gid=1454817404)
2. Determine file formats. 
3. Validate files and formats -- good for checking transfer if checksums are not available.


## Installation

Droid manual: [http://www.nationalarchives.gov.uk/information-management/manage-information/preserving-digital-records/droid/](http://www.nationalarchives.gov.uk/information-management/manage-information/preserving-digital-records/droid/)



*   Download the latest DROID zip file and extract to a folder on your computer.
*   Run DROID from the folder in which it is installed. 
    *   PC -  Double-click on the file called ‘droid.bat’. If you cannot see the droid.bat file check that the ‘Hide extensions for known file types’ box is unticked in your folder options.
    *   Apple - double-click on the file called ‘droid.sh’


## Run DROID



*   DROID will automatically create a new profile for you when it is first started (a blank tab called Untitled-1).
    *   This can sometimes take a little while to fully initialise but once it is ready it should appear as the screenshot does below. You are able to add files to a profile while it is initialising but you will not be able to start running DROID over them until it is ready
    *   You can create multiple profiles and run them at the same time. Each profile will appear in its own tab underneath the toolbar. The profiles can be renamed. Once a profile is created, its settings are fixed.

    

<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: error handling inline image </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>



1. **Add files and folders to a profile** by either clicking ‘Add’ or by selecting Edit>Add Files/Folders.
    *   The box ‘Include subfolders’ is ticked by default. Uncheck this box if you only want to profile the files directly inside a folder and ignore any sub-folders.
    *   If you accidentally add a file or folder that you don’t want to profile, you can simply remove it. 
        *   Note: you can’t add or remove files or folders after a profile has been started – only while you are specifying what you want to profile.
1. **Press ‘Start’ button. **Once you have added all the files or folders you wish to profile you can then run the profile. 
    *   The progress bar will display while the profile is running; this will give you an approximate idea of progress. This is calculated by the amount of files being scanned, it does not account for the size of the files or for files which exist within other files (e.g. zip files).
    *   If required, you can reduce the amount of load DROID is using on your computer, for example, if it is slowing down other applications on your computer. The throttle bar can be moved, allowing you to adjust the speed accordingly. By default it is set to run as fast as possible.
    *   You can pause a profile at any time by pressing the pause button. 
        *   Note: it may take a little while for the pause to take effect, as DROID queues up work which runs in parallel. It must wait for all these tasks to complete before it can pause.
    *   When a profile is paused, you can save, filter, export and create reports on the results generated so far. If a profile is paused, you can resume it by simply re-pressing the start button.
*   **Export results to CSV**
    *   Press the ‘Export’ button. 
    *   Select all the profiles you want to export into a single CSV file by checking the boxes next to them, n.b. if any of your profiles have active filters, then the results will also be filtered
    *   Select ‘export one row per file’
    *   When you are ready, press the ‘export profiles’ button. This will bring up a standard file-save box allowing you to specify where you would like to save your CSV file. Make sure that you select to save the file as a comma separated values file (*.csv).
        *   Note: If you are surveying large amounts of files and wish to use the CSV export you should be aware of spreadsheet application limits. The limits of a workbook for Excel are 1,048,576 rows by 16,384 columns. Be aware that when using functions such as conditional formatting and filtering, these can slow down considerably when surveying a large number of cells. In order to avoid this you can split your DROID profiles into more manageable sizes and then survey the smaller CSVs separately.


## Processing with a DROID spreadsheet



1. Review Droid spreadsheet.
    1. Delete rows containing hidden files using Find and Replace.
        1. These may include database (eg. Thumbs.db) or operating system (eg. .DS_Store) files.
        2. Filenames can also indicate whether a file is hidden/temporary (eg. Filenames that begin with ‘._’ ‘~’ ‘~$’
        3. Be careful to target specific file extensions rather than general keywords which may be used elsewhere in the directory.
        4. Batch find, select, and delete rows using instructions provided here:[ http://excelzoom.com/remove-all-rows-containing-certain-data/](http://excelzoom.com/remove-all-rows-containing-certain-data/)
    2. Edit the file path, including only what would have been included in the original structure.
    3. Address any unusual formats using the EXTENSION_MISMATCH column.
        5. For example, there are multiple files with periods that are causing the format to be stripped.
        6. Use a staging area on your desktop to test extensions to make unknown formats readable.
        7. For now, highlight rows as completed (green).
        8. Add column for notes (first column) and highlight rows that contain notes (yellow).
    4. Review STATUS column for anything other than ‘DONE.’
    5. Remove illegal characters from file names.

DROID User Guide (July 2017)

[http://www.nationalarchives.gov.uk/documents/information-management/droid-user-guide.pdf](http://www.nationalarchives.gov.uk/documents/information-management/droid-user-guide.pdf)

Generating File Format Identification and Checksums with DROID (SAA, July 2016)

[https://cprerc.files.wordpress.com/2016/07/ercm001_generating-file-format-identification-and-checksums-with-droid.pdf](https://cprerc.files.wordpress.com/2016/07/ercm001_generating-file-format-identification-and-checksums-with-droid.pdf)

Internet Assigned Numbers Authority (IANA) List of Official MIME media types

[https://www.iana.org/assignments/media-types/media-types.xhtml](https://www.iana.org/assignments/media-types/media-types.xhtml)

(Further Investigate)

[https://digitalpreservation.natlib.govt.nz/assets/NDHA/Reading/Historical+View+of+format+via+DROIDv4_2.pdf](https://digitalpreservation.natlib.govt.nz/assets/NDHA/Reading/Historical+View+of+format+via+DROIDv4_2.pdf)


