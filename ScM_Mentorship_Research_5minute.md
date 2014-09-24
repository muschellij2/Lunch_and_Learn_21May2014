---
title       : Localization in ICH 
subtitle    : A CT Imaging Pipeline
author      : John Muschelli 
job         : Johns Hopkins Bloomberg School of Public Health
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight  # {highlight.js, prettify, highlight}
hitheme     : hemisu-light      # 
widgets     : mathjax            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
--- .cover #Cover





## CT Images


<img src="Gantry_Corrected.png" style="width:1000px; height:432px; float:right;" alt="Lot of code" >

---


## Brain Extraction!

<img src="../CT_Pipeline/100-318_20070723_0957_CT_3_CT_Head-_SS_Mask_0.01.png" width=400 alt="Data structure", style="float:left;">

<img src="../CT_Pipeline/100-318_20070723_0957_CT_3_CT_Head-_SS_0.01.png" width=400 alt="Data structure", style="float:left;">

---


## Registered Images and Masks

<img src="../CT_Pipeline/native_100-362_20100126_1926_CT_2_CT_ROUTINE.png" width=300 alt="Data structure", style="float:left;">

<img src="../CT_Pipeline/raw_spm_100-362_20100126_1926_CT_2_CT_ROUTINE.png" width=300 alt="Data structure", style="float:left;">

<img src="../CT_Pipeline/roi_spm_100-362_20100126_1926_CT_2_CT_ROUTINE.png" width=300 alt="Data structure", style="float:left;">

---


## Population ICH

<img src="../CT_Pipeline/Figure4_Proportion.png" width=500 alt="Data structure", style="float:left;">
<img src="reoriented_Binary_Sum_Image_histogram.png" width=500 alt="Data structure", style="float:right;">

---



## Voxel-wise Regression

$$
Y_i = \beta_0+\beta_1(v) + \epsilon_{iv}, 
$$
<img src="../CT_Pipeline/Regression_Map_heatcol1_t1.png" width=550 alt="Data structure", style="float:left;">

---

## Regressing on ROI Coverage

$$
{\rm NIHSS}_i = \beta_0 + \beta_1 {\rm Coverage}_i + \gamma_1{\rm Age}_i  +\gamma_2{\rm Gender}_i +\gamma_3{\rm TICHVol}_i + \epsilon_{i}
$$

$$
{\rm GCS}_i = \beta_0 + \beta_1 {\rm Coverage}_i + \gamma_1{\rm Age}_i  +\gamma_2{\rm Gender}_i +\gamma_3{\rm TICHVol}_i + \epsilon_{i}
$$

<img src="Models.png" width=800 alt="Data structure", style="margin:0 auto;">


---

## Regressing on ROI Coverage

<img src="ROI_Results.png" width=550 alt="Data structure", style="margin:0 auto;">

---



