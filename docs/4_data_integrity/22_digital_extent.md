---
layout: default
title: Digital Extent
nav_order: 22
parent: Data Integrity

---

# Calculating Digital Extent
{: .no_toc }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

# Find file count using command line

There are a number of ways to determine file count but the command line should offer the most accurate results. 

**Note: These directions are for use on a Mac.** 

## Open command line dialog box

**On a Mac,** this will be Terminal. You can either search for ‘Terminal’ or open Applications > Utilities > Terminal. 

<iframe src="https://drive.google.com/file/d/1StuSPZyihzzcOpavzz1n9m6qO115ZMOC/preview"></iframe>

## Review Command Line Basics 
See related manual. 

## View file count of folders (excluding hidden files)

The following command will deliver a file count, excluding folders: 

```
   find . -type f -not -path '*/\.*' | wc -l
```

Note: Many of our folders contain a temporary file called thumbs.db. These will need to be deleted to be excluded from the account.  


