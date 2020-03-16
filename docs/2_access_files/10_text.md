---
layout: default
title: Text Files
nav_order: 10
parent: Digital Access Files

---

**_Workflow Type:_ Technical.** This document describes how to create compressed files, and migrate obsolete media. 

**[Link to master document.](https://docs.google.com/document/d/1Jq2VpfHRGNvSzF66e1Ym6StptyC0HOsn0WcskdXWhic/edit?usp=sharing)**

# Text Files
{: .no_toc }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

Creating access files for text documents involves creating a new PDF/A from the original document or conforming to PDF/A standards from an existing PDF, resulting in a read-only PDF-A compliant document.

Currently,  PDF/A-1A or PDF/A-1B are the standard PDF/A types preferred. 

## Single Text Documents

### Using Microsoft Word

**Word (.doc, .docx) and WordPerfect (.wpd) [PC]**

*   Open in Word
*   Select ‘Export’ 
*   Select “PDF XPS Document” > Select “Create PDF XPS”
*   Choose a folder where you would like to save the document and then click “Options” and ensure that “ISO 19005-1 compliant (PDF/A)” is selected.
*   Click “Publish” to save and open.

## Batch Text Documents

### Using Adobe Acrobat Pro

**Word (.doc, .docx), Plain Text files (.txt) [PC], Word Perfect (.wpd)**

_To Create an Action_ (this only needs to be completed once, the action will be saved to the Adobe profile after). 

1. Open Acrobat Pro.
2. Navigate to Tools.
3. Click the “Action Wizard” dropdown.
4. Select “Create New Action.”
5. Under “Files to be processed” make sure default is set to “Add Files…”
6. At left, select Save & Export dropdown, and select save.
7. Click center button (+ →) to toggle this selection to the action pane.
8.  On right, select Save, then “specify settings”
9. Select “Export Files” to alternate format
    1. Select Export to: PDF/A from dropdown.
    2. Hit OK.
10. Hit Save, then input appropriate action name (i.e. “Save as PDF/A”)

_To Use an Action_

1. Select Action from Actions Wizard panel.
2. Use “Add Files” dropdown to select files.
3. Select files to convert, and click “open.”
4. Press Start.


**PDF (.pdf)**

*   Open in Adobe Acrobat Pro
*   Select ‘File’ > ‘Save As Other’
*   Select “Archivable PDF (PDF/A)’
*   Navigate to where you would like to save.
*   Click “Settings” and ensure that “Save as PDF/A-1b” is selected.
*   Click “OK”
*   Click “Save”

**Powerpoint (.ppt, .pptx)**

*   Open in Powerpoint
*   Select ‘Export’ 
*   Select “PDF XPS Document” > Select “Create PDF XPS”
*   Navigate to where you would like to save.
*   Click “Options” and ensure that “ISO 19005-1 compliant (PDF/A)” is selected.
*   Click “Publish” to save and open.


**LibreOffice (unknown file types)**

Libre Office may be used to view unknown text file types and convert them to PDF/A.

*   Open in LibreOffice
*   Select ‘File’
*   Select ‘Export as PDF’
*   In settings, ensure that ‘Archive PDF/A-1a (ISO 19005-1) is selected.

### Using a script

**Wordperfect (.wpd) to PDF/A.**

[https://github.com/acocciolo/file_normalization_tools](https://github.com/acocciolo/file_normalization_tools)

This script will need to be downloaded and installed locally on your Desktop or Documents folder. You can then run the script, following step by step commands, to batch convert all WordPerfect files in a directory. 

# Perform Text Recognition

An example of a text-based document that would need OCR is a scanned thesis. Text recognition should be performed when applicable.

1. Perform Text Recognition (OCR)
    *   Select “Tools” from the “View” menu
    *   Then “Text Recognition” > “In this File” > “All pages” 
    *   Click “OK.” 
2. Highlight text to ensure that all of the text in the file has been recognized.
3. Perform some test searches within the PDFs to further ensure that all of the text in the file has been recognized.
4. Click Save to save the newly OCR’d PDF.
