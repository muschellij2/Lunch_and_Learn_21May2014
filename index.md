---
title       : Stroke Imaging Data- What I have learned
subtitle    : John Muschelli
author      : "@StrictlyStat (github: muschellij2)" 
job         : Johns Hopkins Bloomberg School of Public Health
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight  # {highlight.js, prettify, highlight}
hitheme     : hemisu-light      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
--- .cover #Cover





## Goals

* Registration to a template
* 3D Histogram of Stroke Prevalence
* Longitudinal image registration with CT
* Use some standard or novel methods on CT data for segmentation
* Pipeline

---

## Registration

* Chris Rorden has released a [Clinical Toolbox](http://www.mccauslandcenter.sc.edu/CRNL/clinical-toolbox)
* Has a **CT Template**!
* Uses SPM to do spatial co-registration "Normalization".
* Must mask out the lesion / stroke.

---

## SPM

* Must align to AC/PC line
    * ACPCdetect is on NITRC in ART (automatic registration toolbox) [Here](http://www.nitrc.org/forum/forum.php?forum_id=1927)
    * Chris Rorden has scripts to do this in [SPM8](http://www.mccauslandcenter.sc.edu/CRNL/tools/spm8-scripts)
    * I've done it manually
    * May use Skull Stripping.
* Doesn't use .nii.gz files
* Uses MATLAB

---

## How many patients

* CLEAR IVH - 100 patients
* MISTIE and ICES - 144 patients
* CLEAR III - currently 350 patients (to be 500)
* MISTIE III - 500 patients (just funded)

---

## Data Types

* CT Data - all ROIs are done on axial based CT - also have some saggital and coronal
    * Have follow-up scans that have no blood, but still deformation

---

## What's done - Flow
After Data has been exported from OsiriX:
<img src="CT_Flowchart.png" style="width:400px; height:500px; float:right;" alt="Lot of code" >

---

## CT Image - I have big blood and I can not lie


<img src="Big_Blood_232-512.png" style="width:1000px; height:432px; float:right;" alt="Lot of code" >

---

## Gantry Tilt - Cone heading


<img src="Gantry_Tilt.png" style="width:1000px; height:432px; float:right;" alt="Lot of code" >

---

## Gantry Tilt - It's a Brain!


<img src="Gantry_Corrected.png" style="width:1000px; height:432px; float:right;" alt="Lot of code" >

---

