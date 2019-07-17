---
layout: default
title: Web Archiving
nav_order: 7
parent: Born Digital

---

**_Workflow Type:_ Technical.** This document describes how to track and collect data for The New School Web Archive.

# Web Archiving
{: .no_toc }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

# Administrative

## Archive-It Account Details: [https://archive-it.org/](https://archive-it.org/)

Username: archivist@newschool.edu

Password: [standard password]

_Note: Current subscription started Jan 15, 2018 and will need to be renewed by Jan 14, 2019._

# Stage 1. Appraisal and Selection

## Collection Tracking

ASC tracks web collecting through a Google spreadsheet:

[https://docs.google.com/spreadsheets/d/1CH0lPhcdUxO5ZY0Ls3pE_8HEWcVLpiLmz9HYFrrMfuw/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1CH0lPhcdUxO5ZY0Ls3pE_8HEWcVLpiLmz9HYFrrMfuw/edit?usp=sharing)

Sheet 1: Suggestions to Collect

*   This tab of the tracking spreadsheet collects new recommendations for sites to collect. These can be entered directly by anyone in the Archives department, or added based on input from the TNS community. 

Sheet 2: Active

*   Once the Digital Archivist has created a seed in Archive-It, it may be moved from the ‘suggestions to collect’ sheet to the ‘active.’
*   For ease of use, each sheet is kept in alphabetical order.

Sheet 3: Inactive

*   If a seed has been successfully collected and the site is dormant, or collecting is complete for our purposes, the seed will be set to “inactive” in Archive-it and moved to this sheet.   


# Stage 2. Establish a Web Crawl

The first step of creating a preservation file of a website, is setting up a crawl in Archive-It. A web crawl refers to the process of capturing the content of a website to create a preservation quality format which can be downloaded.

Sites that ASC collects are organized by series in Archive-It. These collections are listed by whether they are Active or Inactive in tabs available within collections.

Active refers to collections with seeds (sites) scheduled to be collected on an ongoing basis, while inactive refers to collections with only inactive seeds (sites that have been previously collected and do not need to be crawled again). If a collection has both inactive and active seeds, it will be marked as “active.” 

Note that collections must be designated “Active” and “Inactive,” through a drop-down field within each collection Overview. These categories are not assigned automatically.

## Step 1: Add a new seed

1. Select ‘Collections’ from the homepage.
2. Select related collection from ‘Active’ or ‘Inactive’ collections, or create a new collection.
    1. If the seed belongs to a collection currently set as ‘Inactive,’ the collection will need to be updated to reflect the new, active seed.
3. Within the collection, select “Seeds” tab.
4. Click Add Seeds.

## Step 2: Define parameters of the seed

1. Add URL 
    1. Archive-It will give immediate feedback as to whether the added seed is valid. If you try to add a seed that already exists, or another issue arises, a caution icon will appear, and the hover message will specify the issue. 
    2. Details on formatting social media or specific types of urls can be found here: [https://support.archive-it.org/hc/en-us/articles/208001336-Scoping-guidance-for-specific-types-of-sites](https://support.archive-it.org/hc/en-us/articles/208001336-Scoping-guidance-for-specific-types-of-sites) \

2. Set ‘Access’
    3. Choose whether the site will be part of the public facing Archive-It TNS account ([https://archive-it.org/home/newschool](https://archive-it.org/home/newschool)) or have restricted access based on the status of the collection. The seed should remain ‘Private’ until a crawl has been saved to Wayback.
3. Set ‘Frequency’
    4. Frequency is ideally established by assessing how often a site is updated, the type of content being captured, and the purpose for preserving the content. Another factor that may also determine capture frequency is the data plan in place, which may restrict number of captures. 
        1. Example A: The inactive site of a newly retired faculty member will be captured One-Time.
        2. Example B: The New School website, updated every 1-3 months, will be captured bi-annually. 
1. Set ‘Seed Type’
    1. **Standard**: This will crawl all pages (in-scope) and variations of the URL.
    2. **Standard Plus External Links** (**Standard +): This will crawl all pages (in-scope) and variations of the URL plus one layer of pages linked from the site (outside the scope).
    3. **One Page:** This will crawl a single page of seed site.
    4. **One Page Plus External Links (One Page +):** This will crawl a single page of the site plus one layer of links from this page (inside or outside the scope)..


## Step 3: Perform Test Crawl 

After you add your new seeds, you may run your first crawl. There are two types of web crawls: 

*   **Test Crawl** Deletes data after 60 days, unless saved.
*   **Production Crawl** Auto-saves data to the Archive-It account.

**When crawling seeds for the first time, it is important to perform an initial test crawl.** 


*   Production crawls will automatically add data to an account, so test crawls are an easy way to get an accurate indication of how your seeds will crawl, archive, and replay before you expend any of your account's data budget. They allow you to review and plan for the crawl duration, scoping rules, and other factors that can make your future "full production" crawls as successful and efficient as possible.

 To do this, navigate to the Collection or Group of seeds that you wish to collect: \


1. Select all or some of the seeds within the collection/group to crawl 
2. Click Run Crawl.
3. The Pop Up window will provide you with a series of choices to dictate the extent of your crawl. 
    2. Select Test Crawl. Optional: assign a document limit. 
    3. Optional: Assign a data limit. 
    4. You _must _assign a time limit. 
*   For our purposes, most crawls will have a time limit of 7 days.
*   Decisions on time limits should be estimated based on the extent of the data being collected.
*   Keep in mind that Archive-It will not run multiple crawls at one time.
    5. Finally, you may select whether to _only_ crawl PDFs within the scope of your seeds.
    6. All limitations that are added to a crawl may further narrow the scope defined by your individual seeds.
*   For example, if you assign a relatively short time limit to a crawl with an expansive scope, the crawl will end before all related data is collected, which may lead to missing data or display issues in Wayback.
*   Production crawls may be continued if they “time out” but test crawls may not.
1. Run the crawl. 
2. Check Test Crawl Report.
    1. Once your test crawl has completed, you can find it's reports listed in either the "Crawls" section of the web application, as you would any full production crawl, or else from the "Crawl Reports" or "Test Crawls" lists in the given collection's Crawls tab.
    2. Select a crawl report under ‘Crawl ID.’
    3. Navigate to Seeds tab.
    4. Perform Quality Assurance per directions below.


# Stage 3. Perform Quality Assurance (QA) and Analysis

It is necessary to perform quality assurance (QA) to ensure that the desired content has been collected, that needed content has not been blocked, that information is no longer queued and that the WARC file displays correctly in Wayback.


## Step 1. Check Crawl Reports

The first step of completing a QA is to analyze the crawl reports for issues.

You may access a crawl report from within a collection, or via the “Crawls” tab on the Archive-It toolbar. An individual report can be accessed by clicking its unique Crawl ID number.

1. Identify that your crawl finished successfully from the status listed in the **Crawl Overview Report**. The example above is marked as “Finished.”
    1. If a report reads “Finished - Time Out,” this means that the time limit parameter was hit before successfully completing the crawl. Most likely, the seed should be evaluated and settings changed. 
2. Click on “Seeds” to review the **Seeds Report**. \

3. Confirm that each Seed’s status appears as “crawled.”
4. Click “Hosts” to check the **Host Report.**
5. Review the information in your crawl's [Hosts report](https://support.archive-it.org/hc/en-us/articles/208333883-How-to-read-your-crawl-s-hosts-report) in order to determine if any valuable hosts were blocked from crawling by robots.txt exclusions or deemed as outside the scope of your crawl. Queued documents that do not point to a [crawler trap](https://support.archive-it.org/hc/en-us/articles/208332943-Identify-and-avoid-crawler-traps-) may indicate that the time, document, or data limit on the crawl should be extended in order to capture missing elements. Some scoping changes can be made directly from the Hosts report, see [Modify scope and run patch crawls from your repor](https://support.archive-it.org/hc/en-us/articles/208333823-How-to-modify-scope-and-run-patch-crawls-from-your-report)t.
    *   **Check the blocked column to identify if any parts of a host report have been blocked by a robots.txt file.**
    *   Check for queued documents and identify whether they are necessary
        *   Rerun crawl with longer time, file count, etc. if it was a Test Crawl
        *   Continue the crawl for a specified amount of time, if it was a Production Crawl.
*   Check if documents were blocked by robots.txt & ID whether these were necessary
    *   Add rule that allows us to ignore robots.txt blacks in the future

## Step 2. Enable Wayback QA

Access your collected pages in Wayback through two means:

1. Access the Wayback link through your individual Seed Reports.
2. Search or browse your collected pages through the Archives tab in the Archive-It toolbar.
*   Discovers missing documents from already captured pages.
*   Only looks for missing docs on the page that you are viewing.

## Step 3. Check pages in Proxy mode

*   View archives site in proxy mode in your browser
    *   Allows you to replay the documents that were archived without the influence of the live web
    *   Only available for sites beginning with http, _not_ https
    *   Not available for most social media sites
    *   May enable by using the Firefox browser extension
        *   (NOTES in Help Center)

_Troubleshooting_

### Patch Crawls

*   Will only crawl the individual documents selected from the list.
*   Will not follow links off documents.
*   Will not capture embedded content in docs.
*   Don't adhere to collection of seed scoping rules.
*   Data avail 24 hours after crawl finishes.

### No Data or additional missing documents?

*   Check that host report. If nothing is blocked or queued, then…
*   Enable QA. If nothing important is missing then…
*   Crawling the page as a seed
    *   By adding a specific page as a seed, you should be able 
    *   Umbra - Runs alongside Heritrix on only the first page of each seed. Can capture embedded and dynamic content like carousels and video.

Walk-though QA process:[ https://support.archive-it.org/hc/en-us/articles/208333833-Quality-Assurance-Overview](https://support.archive-it.org/hc/en-us/articles/208333833-Quality-Assurance-Overview)

---------

# Further Documentation needed: 
* Steps for transferring file to Preservation server
* Creation of metadata for captured sites

Note: WARCs currently stored in Central_Kellen_share/preservation/Archive_It_WARCs

Additional steps for getting things up-to-speed:

1. Locate HTTrack files from 2016 & earlier
2. Locate legacy PDFs downloaded 
3. Determine how to collect older TNS sites in archive.org


# Resources

* Archive-It 
[https://support.archive-it.org/hc/en-us](https://support.archive-it.org/hc/en-us)

* Archive-It Help Center
    *   Mary Haberle (mhaberle@archive.org) has helped in the past.
    *   Requests can also be submitted via the [Help Center](https://support.archive-it.org/hc/en-us/requests/new) 
* [Archive-It Video Curriculum](https://support.archive-it.org/hc/en-us/articles/216489103-Archive-It-Video-Curriculum-#postcrawl) 

* The Web Archiving Life Cycle Model, Archive-It 

[http://ait.blog.archive.org/files/2014/04/archiveit_life_cycle_model.pdf](http://ait.blog.archive.org/files/2014/04/archiveit_life_cycle_model.pdf)

* Web Archiving Section of SAA

[https://www2.archivists.org/groups/web-archiving-section](https://www2.archivists.org/groups/web-archiving-section)

* Code4Lib
[https://code4lib.org/about](https://code4lib.org/about)

* Getting started with web archives: 2018 beginners’ workshop
[https://www2.archivists.org/groups/web-archiving-section/getting-started-with-web-archives-2018-beginners%E2%80%99-workshop](https://www2.archivists.org/groups/web-archiving-section/getting-started-with-web-archives-2018-beginners%E2%80%99-workshop)

* Archive-It offers a full Video Curriculum through their Help Center at:
[https://support.archive-it.org/hc/en-us/articles/216489103-Archive-It-Video-Curriculum-](https://support.archive-it.org/hc/en-us/articles/216489103-Archive-It-Video-Curriculum-)

_Collection Development Policies/ University Web Archives_

* North Carolina State University (NCSU)
[https://ncsu-libraries.github.io/web-archiving-docs/](https://ncsu-libraries.github.io/web-archiving-docs/)


* Columbia University
[https://library.columbia.edu/bts/web_resources_collection.html](https://library.columbia.edu/bts/web_resources_collection.html)


* Stanford University
[http://library.stanford.edu/projects/web-archiving/collection-development](http://library.stanford.edu/projects/web-archiving/collection-development)

