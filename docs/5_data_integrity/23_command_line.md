---
layout: default
title: Command Line Basics
nav_order: 23
parent: Data Integrity

---

# Command Line Basics 
{: .no_toc }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Review Command Line Basics 

* “Print Working Directory” - view your current location

```
    pwd 
```

* Change your directory (DIRECTORY_NAME represents the folder you would like to move _into_)

```
  cd DIRECTORY_NAME
```

* Move up a directory

```
  cd ..
```

* View all files and folders within the directory where you are located


```
   ls
```

* View file count of folders (excluding hidden files)

The following command will deliver a file count, excluding folders: 

```
   find . -type f -not -path '*/\.*' | wc -l
```
* Unlock files in a directory

```
   chflags -R nouchg DIRECTORY_NAME
```