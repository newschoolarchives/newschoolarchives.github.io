---
layout: default
title: Imports 
nav_order: 15
parent: Collective Access

---

**_Workflow Type:_ Technical & Communication.** This document describes how to prepare and execute imports to Collective Access. 

[Link to master document](https://docs.google.com/document/d/19bBGWOMLcgAQ-QFdRv15cLOwNHmpjUJTzbMZQbNptpo/edit)

# Imports
{: .no_toc }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

# Overview

Batch Imports only occur when more than 10 digital files need to be uploaded to Collective Access. To read more about this policy, review [Workflow: Scan Request Processing](https://docs.google.com/document/d/1QFmm7WE7VZE7eiDa2X7ECUW-AXxvXZSACsivlVrgT2w/edit).


# Batch Imports


## Stage 1. Import Data


### Step 1. Review spreadsheets for import  



*   Guidelines for formatting metadata can be found in the adjacent tabs of the import template.
*   Files and data template for import will be placed in a folder within Staging_active that is titled by the scan request ID number, or a relevant collection identifier. 
*   When the folder contents are prepared, ‘_READY_FOR_UPLOAD’ will be appended.  
*   Dropdowns and columns with comments that are not part of the mapping should be removed before importing.


### Step 2. Move Preservation Files 

*   TIFFs and non-access formats go to corresponding collection folder in K:\preservation


### Step 3. Import data into CollectiveAccess 

*   Login to the backend: [http://digitalarchives.library.newschool.edu/admin](http://digitalarchives.library.newschool.edu/admin)
*   Choose "Import" from the top menu and then select "Data" from the dropdown. 
*   There are three import templates used: 
    *   “Internal Scan Request Mapping” - standard import
    *   “Thesis Mapping” - thesis import 
    *   “AV Mapping 2019” - audiovisual import
*   It’s good practice to perform a ‘dry run’ of the import first to see if the spreadsheet data needs to be edited.


### Step 4. Create a Set  

*   Once the import has been completed, create a set to use for review within the department.
*   Find > Objects > Search on collection identifier then ‘Refine’ results by selecting records with restricted access (new records import automatically as ‘restricted’)
*   Save 'Set' with newly imported records as ‘MM-DD-YY [Collection ID] Import.’ 
*   Confirm that the data looks correct across records. If changes need to be made, consider if they can be done by batch, manually, or if it would be preferable to delete and re-import the data. If so, this should be done before adding media. 


## Stage 2. Import Media 


### Step 1. Transfer Files through FTP

[PC]



*   Open Windows program Secure Shell Client.

*   If logging in for the first time, set up a new profile: 
        *   Click Profiles > Add Profile
        *   Name the profile after the administrator. Press okay.
        *   Host name: digitalarchives.library.newschool.edu
        *   User name: TNS web ID of the administrator with access (in this example: adm_martinezk)
        *   Port number: 22
*   Select Window > New File Transfer.
*   In new window, add **/collectiveaccess/app/public_html/admin/import/** to navigate to the collective access directory.
*   Create folders for content to be imported.
*   Remove contents once the import process is complete. 

[Mac]



*   Open Transmit app
*   Input credentials 
*   Click file location at the top of the right pane and navigate to digitalarchives.library.newschool.edu > collectiveaccess > app > public html > admin > import


*   Drag and drop files to be imported. 


### Step 2. Import into CA



*   Login to CA at [http://digitalarchives.library.newschool.edu/admin/](http://digitalarchives.library.newschool.edu/admin/)
*   Select Import > Media
*   Select folder created in the import directory 
*   Confirm settings before importing:
    *   Import mode: “Import only Media that can be matched with existing records.”
    *   Select object type.
    *   Choose access settings.
    *   Show advanced options > Select match using directory name or filename
*   Execute media import


### Step 3. Update Featured Topics, if relevant


### Step 4. Move Access Files



*   JPEGs and PDFs go to corresponding folder in K:\working_files\Dig_images_access


### Step 5. Checklist for Completed Import 



*   Check relationship types to see that description is accurate for non-designer or non-commissioner roles
*   Make any new entities accessible to public through batch change 
*   Review media for missing data
*   Check that PDFs can be searched, if applicable 
*   Check that media plays correctly, if applicable 
*   Check ‘minimum standards met’ for all records through batch
*   Check that dates are correct for non YYYY formats 
*   If new collections are added, update AT as needed 


### Step 6. Share following details with supervisory archivist:



*   Records are all associated with a set (if applicable)
*   Preservation files have been moved
*   Access files have been moved
*   Filemaker fields have been updated
*   Data spreadsheet has been moved


## Stage 3. Update Archivists’ Toolkit 



*   _See ‘Adding Digital Object Links’ in AT Processes_


# **Batch Updates**


### Step 1. Create a Set

Select the records you would like to include by performing a search. In this example, we search on the base identifier. 



*   In the upper right corner, select ‘Find’ > ‘Objects’
*   Search: [NS021201] > Click ‘Search’ 
*   After results are returned, select ‘Set Tools’ from the left menu
*   Select ‘Create Set’ and use the dialog box to name your set. You’ll see a dropdown menu that allows you to add records from the search results, or from checked records. Clicking the box ‘Open set for batch editing’ will automatically open batch editing for this set. If that option is selected, the next step can be skipped. 


### Step 2. Batch Edit a Set



*   In the upper right menu, select ‘Manage’ and then ‘My sets.’ Locate your new set and select the files icon in the ‘# Items’ column to batch edit the records.

 
