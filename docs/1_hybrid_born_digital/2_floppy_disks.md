---
layout: default
title: Floppy Disks
nav_order: 3
parent: Hybrid & Born-Digital Media

---

**[Link to master document.](https://docs.google.com/document/d/1xiW_uWBhi3fzp_IHT_B9strGWNVOXOUEN5NbwXxug1g/edit?usp=sharing)** [Last Updated: Aug 23, 2019]

# Disks
{: .no_toc }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

# Stage 1. Appraisal 
The processing archivist will transcribe disks and appraise the contents using Quick View Plus. Directions for processing will be added to the [Disk Inventory Spreadsheet](https://docs.google.com/spreadsheets/d/1mNAgjEYjdHNR-sLehjg5YafFLu3W-U-SWUbc39D55-8/edit#gid=426583852)

For a full description of the appraisal process, see the [Removable Media](https://newschoolarchives.github.io/docs/1_removable_media) overview. 

# Stage 2. Create a Disk Image and Extract Files using Bitcurator
The Bitcurator station (non-networked computer) will be used for the transfer of floppy disks.

For more information, see the BitCurator manual: [http://distro.ibiblio.org/bitcurator/docs/BitCurator-Quickstart-v2.pdf](http://distro.ibiblio.org/bitcurator/docs/BitCurator-Quickstart-v2.pdf)


## Step 1. Create forensic disk image

*   Before inserting floppy disk into USB reader: 
    *   **Set the BitCurator environment to read-only.** Look in the top right corner of the BitCurator environment and locate a small icon of a disk drive. Check to make sure that this icon is green, indicating that any new disk will be mounted as read-only. If the icon is red, click on it and choose read-only from the dropdown options. 

    *   **Ensure that the floppy disk is write protected.** Do this by checking that the appropriate tab per disk type is open:

	![alt text](https://www.dummies.com/wp-content/uploads/0-7645-0361-8_1301.jpg)

    Source: https://www.sciencedirect.com/topics/computer-science/write-protection

	*   Open Guymager (in “Imaging and Recovery” folder on desktop).
        *   If a password is requested: bitadmin
    *   Insert floppy disk in drive.
    *   Click “Rescan” button in top left corner of window.
    *   A new row should appear reading “/dev/sdb” under “Linux device” and probably 1.5 MB under Size: select this row.
    *   With row highlighted, right click and choose “Acquire Image.”
        *   Select ‘Expert Witness format.’
        *   For “Case number” enter accession ID (ex: 2014KA01) or collection ID.
        *   For evidence number enter disk number (ex: D004, D005, etc).
        *   Under “Examiner” put your own name (enter it the same way every time).
        *   Under “Description” write “no label” if the disk is unlabeled. If the disk has a label write “Label:” followed by whatever is written on the disk, for example “Label: Newsletter October 1994 Issue December 1984 Issue”.
        *   Click “...” button from the dropdown menu under “Look in:” choose “/home/bcadmin/Desktop/Disk Images” then click the “Choose” button.
        *   Make sure “Calculate MD5” and “Verify image after acquisition” are checked, then click the “Start” button.

## Step 2. Generate Reports

*   Open ‘Forensics and Reporting’ folder
*   Open 'BitCurator Reporting Tool’
*   Select 'Fiwalk XML' tab
*   Under 'Image File' navigate to the disk image
*   Under “Output XML file” select the same directory as the disk image
*   Input identifier for the new filename 

Note about fiwalk report:  <alloc>1</alloc>  = 1 means that this an allocated file, not a deleted file, or signature file. 

For detailed descriptions of each fiwalk metadata element: [https://github.com/BitCurator/bitcurator-distro-metadata/blob/master/csv/dfxml.csv](https://github.com/BitCurator/bitcurator-distro-metadata/blob/master/csv/dfxml.csv)


## Step 3. Extract Preservation Files

*   Create a folder for each disk with name corresponding to the assigned identifier on the desktop of BitCurator (the case number/accession number followed by an underscore then the evidence number/disk number (ex: 2014KA01_D001).
*   Navigate to Forensics and Reporting folder.
*   Select BitCurator Disk Image Access tool.
*   Click on the folder icon, ‘Open Disk Image’ in the toolbar. Select disk image file.
*   A directory of files contained in the disk image will be displayed
    *   Entries in bold are directories.
    *   Entries in red are deleted/unallocated files

<iframe src="https://drive.google.com/file/d/1uMgp8kI_3m4I3Fl6gtUPtYzXeok2T1Xi/preview" width="640" height="480"></iframe>

*   **Select files manually or by clicking Edit > Select Allocated Files** (this will only select files that are not deleted/unallocated). 
    *   Keep in mind that files may be nested in directories, if selecting manually.
    *   System files (ie. FAT12, MBR, etc.) can be deleted. 
*   **Export files.**
    *   Select Export icon (paper plane to the left of the Cancel icon).
*   Review that exported files are in the desired location

pages 47-49 of the BitCurator Quickstart Guide:[http://distro.ibiblio.org/bitcurator/docs/BitCurator-Quickstart.pdf](https://wiki.bitcurator.net/downloads/BitCurator-Quickstart.pdf)

## Step 4. Transfer Files to PC for processing

*   **Transfer folder of extracted files using an external harddrive.**
    *   Change the Bitcurator disk drive icon in the top right corner to "writeable" from the dropdown to allow files to be transferred onto the drive once it is mounted.
    *   Connect the external hard drive to a networked machine. It should automatically begin a virus scan. If not, open Symantec Endpoint Protection and initiate a scan of the drive before transferring any files onto your computer or the shared drive.
    *   Use Exactly to transfer files from the harddrive to the staging server where file normalization will take place. 

# Stage 3. Create Access Files
[See related manuals](https://newschoolarchives.github.io/docs/3_access_files).


# Stage 4. Contact Processing Archivist for a final review of content. 

