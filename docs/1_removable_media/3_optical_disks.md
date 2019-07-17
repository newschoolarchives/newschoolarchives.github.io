---
layout: default
title: Optical Discs
nav_order: 4
parent: Removable Media 

---

**_Workflow Type:_ Technical.** This document describes how to process optical discs after they have been appraised. 

# Optical Discs
{: .no_toc }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

# Stage 1. Appraisal 
The processing archivist will transcribe disks and appraise the contents using Quick View Plus. Directions for processing will be added to the [Disk Inventory Spreadsheet](https://docs.google.com/spreadsheets/d/1mNAgjEYjdHNR-sLehjg5YafFLu3W-U-SWUbc39D55-8/edit#gid=426583852)

# Stage 2. Extract files 

## **DVDs & CDs with data (administrative files)**

### Step 1. Copy files to server 

[Windows:]

*   After inserting disc and **performing a virus scan using Symantec Endpoint**, navigate to the Disc Drive in a Finder Window, select all content, right click and copy/paste files to Staging server. 
*   TeraCopy will conduct the file transfer and verify that each file has been successfully copied.

## **DVDs/CDs Formatted for Audio**

   *   Note: Audio media may appear as a series of files with the type CD Audio Track [.CDA files].  These will not copy successfully from the disk and must be extracted using EAC.
   
<iframe src="https://drive.google.com/file/d/14FSKGDrv9vruG7m_PTpwARHYFoapLMCR/preview" width="640"></iframe>

[Windows]

### Step 1. Extract WAV Audio Files

*   Open Exact Audio Copy
    *   Verify that software configuration is correct as described in ‘[Configuring Exact Audio Copy](https://docs.google.com/document/d/1HGi-yu-xpfE3Eji0NGsDhBX1tqfs8EfBEXtlIE2xabs/edit#bookmark=id.i3g51pfcw2v5).’
*   Go to _Database > Get CD Information From > Remote Metadata Provider_. EAC will attempt to download information and if there are multiple results, you will be prompted to double-click on the correct one to save.
*   If no information on audio CD was provided by EAC, assign a title, artist (i.e., the collection creator, unless there is a clearly identified individual or group who is responsible for the recording and/or holds copyright) and year. If applicable, you may also add a genre as well as performer (especially if others have contributed to the recording) and composer.  If known, you may also add titles to the individual tracks.

<iframe src="https://drive.google.com/file/d/1m9foX_VD8PloIgwJsGPcJHbWzAQq63Ue/preview" width="640"></iframe>

*   After making sure that the check boxes next to all tracks are filled, select _Action > Copy Selected Tracks > Uncompressed_.   

*   When prompted, browse to the folder where you will save the files.
*   EAC will begin copying the audio tracks, displaying progress and any errors in a window; upon completion, you will be presented with a status report and notified of any errors. Click "OK" to proceed.
*   Go to _Action > Create CUE Sheet > Multiple WAV Files (with corrected gaps)…_; save the resulting file (which will automatically be named with the CD title) alongside the WAV files and log. This CUE sheet (plain text) will contain all the metadata you entered as well as information on track listing and timing.
*   The resulting files will serve as your uncompressed, master WAV files for preservation and may be compressed into MP3 Access Files.

### Step 2. Compress WAV Files into MP3 Files

*   Open EAC, and verify that software configuration is correct as described below.
*   Go to EAC > Compression Options >External Compression
    1. select “Use external program for compression”
    2. insure that the Program and Path is correct
        1. Upon install, EAC recommends LAME.exe for MP3 encoding
        2. This encoder is not included in the EAC package due to patent and licensing issues.
        3. Lame.exe may be downloaded from a number of sites including [http://rarewares.org](http://rarewares.org)
*   Select “320 kBit/s” from the Bit rate drop-down menu.
    1. 320 kBit/s is [approximately the bit rate at which the human ear cannot recognize the difference between CD audio and a digital file](https://computer.howstuffworks.com/mp32.htm).
    2. MP3 files are around 1.5 MB per minute.
*   The “Additional command-line options:” line must be populated for successful external compression in LAME.exe. A sample command line reads:

-V 0 --vbr-new --ta "%artist%" --tt "%title%" --tl "%albumtitle%" --tg "%genre%" --ty "%year%" --tn "%tracknr%" --tc "%comment%" %source% %dest%

Full command line options may be found at:

[https://wiki.hydrogenaud.io/index.php?title=EAC_Compression_Options](https://wiki.hydrogenaud.io/index.php?title=EAC_Compression_Options)

*   Important: Make sure that “Delete WAV after compression” is _un_checked_. If this box is checked, your working uncompressed WAV files will be deleted, and you may be forced to re-transfer files from the disk.

<iframe src="https://drive.google.com/file/d/1jgPvnKx-fToElOyo3HJ0o9Z_PYmcer1p/preview" width="640"></iframe>

*   Select uncompressed WAV files, and drag them into the EAC window.

<iframe src="https://drive.google.com/file/d/1_Rx99DZuODQcuqtu0AbKZU2LpCMUjlyw/preview" width="640"></iframe>

*   In the pop-up browser, navigate to the destination for your compressed MP3 files.
*   When compression is complete, click OK.

*   After creating audio access files, playback audio for a few seconds at the beginning, middle, and end to spot check quality, audio, and rule out other potential file issues.
*   Transfer Access and Preservation files to the appropriate locations using TeraCopy.

### Step 3. Configure Exact Audio Copy (EAC) for Audio File Extraction and Creation

[Windows]

*   Open Exact Audio Copy (EAC)
*   Go to EAC > EAC Options > Character Replacements. Make sure that quotations marks (“), carets (^) and percent symbols (%) are not replaced by another character:

<iframe src="https://drive.google.com/file/d/1D9CRQ0ACirKp8RmrZkMK6ZrGL4Ml0iZG/preview" width="640"></iframe>

*   Go to EAC > EAC Options > Write. Disable the option to use all uppercase characters on writing: 

<iframe src="https://drive.google.com/file/d/1rDQaCpKBjffnDIv92MtKwb7S0FpWIHic/preview" width="640"></iframe>

*   Go to EAC > EAC Options > Tools. Enable options to write a status report after extraction and to append a checksum to this report.

*   Go to EAC > Compression Options > Waveform. Select “Microsoft PCM Converter” for Wave Format and “44.100 kHZ, 16 Bit, Stereo” for Sample Format:

*   Go to EAC > Metadata Options > Metadata Provider. Select “freedb Metadata Plugin” from the menu. Under the options, configure EAC to “Never” search for cover images or lyrics.

*   Go to EAC > Metadata Options > freedb. Enter your TNS email address.

## **DVDs/CDs Formatted for Video**

_Note: One way to recognize video media is by its AUDIO_TS and VIDEO_TS folders:_

<iframe src="https://drive.google.com/file/d/1z6PbU-mhos7txU6QnIdARruR4o9Lqehb/preview" width="640"></iframe>

### Step 1. Create MP4 Files Using Handbrake

*   Open Handbrake 
*   Select  ‘Open Source’
    *   Add DVD or File 
        1. Under “Source Selection,” select the ‘File’  
        2. Select the D: drive, then hit ‘Open’ 
            * the “Titles” menu will show if there is more than one video on the disc
            <iframe src="https://drive.google.com/file/d/1u2C2TRW4wioC4VIWdkndbW0updZBcvuP/preview" width="640"></iframe>
        3. Select video files through ‘Source Selection’ or by dragging the file into the grey box in the center of the new HandBrake window.
        4. Confirm Handbrake Output File Settings
            <iframe src="https://drive.google.com/file/d/1lx6AfnxHoBaiWy0NcXt5gVEO1_P1YKEd/preview" width="640"></iframe>
            * Go to Tools > Preferences and select the “Output Files” menu. Enable “Automatically name output files” and browse to the appropriate folder for the default path. Under “Format,” do not change {source}-{title} and make sure the “Always use MP4” option is selected.
            * Note: If you're working with a non-commercial DVD and, as a result, "Automatically name output files" results in a non-unique default name to your MP4 file, change the name to the item's disk identifier, e.g., "Format: 2014NS06_D001" (without the {source} or {title}).
            * If you're working with a non-commercial DVD (as above) and it has multiple tracks, change the name to the item's disk identifier followed by the title, e.g., "Format: 2014NS06_D001-{title}" (without the {source}).
        5. Select Video Settings
            * Navigate to the Summary Tab
            * Make sure that Format is set to MP4.
            * Make sure that Align A/V Start is selected.
            * Navigate to the Video tab, and select the appropriate quality settings as outlined by winxdvd.
            * Video Codec: H.264
            * Framerate (FPS): “Same as Source” “Variable Framerate”
            * Optimise Video, 264 Preset: “Very Fast”
            * Constant Quality: 20 RF
        6. Select Audio Settings
            * Navigate to the Audio tab, and select the appropriate quality settings.
            * Select the Audio tab and AAC (ffmpeg) Codec. 
             * Choose: 
                * 48.000 Hz Sample Rate. 
                * Stereo for Mixdown. 
                * Choose at least 160 for your audio Bitrate. If you encounter artifacts or other audio issues, increase bitrate to 320 or higher.
        7. Check Dimensions
            * Navigate to the Dimensions tab, and ensure that dimensions (Width and Height) match that of the source video, or, if you are reducing size for compression, ensure that you retain the original ratio and no unnecessary cropping occurs. For example, this can be done by using an online [Aspect Ratio Calculator](https://calculateaspectratio.com/). 
        8. Recheck output file name and location
            * Before executing encoding or adding to queue, check “Save As” destination and filename in the bar below the media. This field will automatically populate with the settings you selected earlier under Tools > Preferences > Output Files, but you may change manually.
        9. Add to Queue
            * Click “Add to Queue” or (if there are multiple titles on the disk) click the arrow to open an option to “Add all.” 
        10. Start
            * Click “Start”; Handbrake will go through the queue and provide progress information near the bottom of the window. It may take a relatively long period of time for the conversion process to complete. It may be necessary to adjust the power settings on your workstation so that it will not sleep.
        11. Check New Files
            * After creating video access files, playback video for a few seconds at the beginning, middle, and end to spot check quality, audio, and rule out other potential file issues.

**Recommended Output Settings Mp4**

Source: [https://www.winxdvd.com/resource/fix-handbrake-video-quality-poor-problem.htm](https://www.winxdvd.com/resource/fix-handbrake-video-quality-poor-problem.htm)

**Continuing Research**

*   Handbrake will only export MP4 or MKV files
    *   Through upping the “Constant Quality” in export, we can create “lossless” MP4 or MKV files, which will contain more info than their eventual access counterparts.
        *   Continue Research --- These “Lossless” MP4s are not playing back in Windows Media Player, while the compressed access versions work fine.

From [Preserving Moving Pictures and Sound, by Richard Wright](https://www.dpconline.org/docs/technology-watch-reports/753-dpctw12-01-pdf/file):

“Ideally video would be stored uncompressed in a professional, open standard wrapper. MXF is recommended, but MOV and AVI are also used. AVI cannot be used on professional broadcast video with embedded timecode, or the timecode will be lost. Lossless compression is also used in major audiovisual archives, specifically JPEG 2000.”

**Additional Compression for Collective Access**

On occasion, larger/longer MP4 Videos may need to be compressed further to facilitate better load time through Collective Access. To accomplish this, you may wish to adjust the video dimensions to match the playback window on the Digital Archives site. 

Suggested Settings:

<iframe src="https://drive.google.com/file/d/1vsW50tv2NorCSlv9OQqWptCe8Tb-FE5H/preview" width="640"></iframe>

<iframe src="https://drive.google.com/file/d/13nlsOL4Otwc6m8OtSOvAr7DuR2DIUDqb/preview" width="640"></iframe>

<iframe src="https://drive.google.com/file/d/1hStEJHSQObzIHU0D0igihuGv_ITNKYuF/preview" width="640"></iframe>

**Special Format - .rm files** 
https://walkerart.org/magazine/how-to-convert-real-media-video-into-h-264-mp4

# Stage 3. Create DROID Report
[See related manual](https://newschoolarchives.github.io/docs/5_data_integrity/18_droid.html).