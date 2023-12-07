---
layout: page
title: Our Methods
---


# Project Context 
The HTT project is a collaborative project that **crowdsources pathologist annotations.** The annotations we are collecting are estimates of the density of stromal tumor-infiltrating lymphocytes (sTILs) in breast cancer. sTILs are a prognostic biomarker ([Salgado2015_Ann-Oncol_v26p259](https://doi.org/10.1093/annonc/mdu450), [Loi2019_J-Clin-Oncol_v37p559](https://doi.org/10.1200/jco.18.01010)). 

This project will additionally produce statistical analysis tools to evaluate algorithm performance given the variance in the ground truth. 

# Our Methods 

### Pilot Study
For our pilot study, we digitized 64 glass slides of stained ductal carcinoma core biopsies prepared at a single clinical site. A collaborating pathologist selected 10 regions of interest (ROIs) per slide for evaluation. We created training materials and workflows to crowdsource pathologist image annotations with two modalities: an optical microscope, **eeDAP**, an Evaluation Environment for Digital and Analog Pathology, and two digital platforms, **caMicroscope,** and **Path Presenter**. (More information in the next section). The annotation workflow asks the pathologist to evaluate the ROI type, make a decision on whether the ROI is appropriate for estimating the density of sTILs, and if appropriate, estimate amount of tumor-associated stroma in the ROI and the density of sTILs in the stroma. The pilot study data are publicly available [HERE](https://github.com/DIDSR/HTT). 

### Pivotal Study
For our current pivotal study, we used what we learned in the pilot study (ref: clearr-ai) to update the study design to reduce the high degree of pathologist variability that we experienced in the pilot study.  We currently have over 80 (check this number) TNBC slides from 2 collaborating sites and are still sourcing more slides and images to add to the study.  **expand this...**

#  Technologies Used in this Project 
### Digital Platforms 
We have two digital platforms for viewing and annotating whole slide images: [caMicroscope](https://wolf.cci.emory.edu/camic/htt/login.html) and [PathPresenter](https://htt.pathpresenter.net/). Pathologists can log in from anywhere in the world and annotate images using these web-based viewers. 

Leadership from caMicroscope and PathPresenter are collaborators on this project and have supported the development of controlled and standardized workflows to select and evaluate ROIs.

### Microscope Platform  
The optical microscope platform uses a hardware and software system called eeDAP, an Evaluation Environment for Digital and Analog Pathology [Gallas2014_J-Med-Img_v1p037501](https://www.doi.org/10.1117/1.JMI.1.3.037501). The eeDAP system registers the live-camera view of the microscope slide with a digital scan of the slide taken with a whole slide imaging system. The eeDAP system is programed to automatically move the motorized stage to pre-specified regions of interest (ROIs) within a slide, so that we can collect data in microscope or digital mode. Annotations collected on the microscope (the reference standard device) are free of degredations from slide digitization.
