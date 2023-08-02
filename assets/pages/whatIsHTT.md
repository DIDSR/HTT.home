---
layout: page
title: What is HTT?
subtitle: Background and Publications
---

This page tells you a little bit about the project.

# Our Goal
The goal of the High-Throughput Truthing (HTT) project is to produce a **validation dataset** established by pathologist annotations for artificial intelligence algorithms analyzing digital scans of pathology slides: data (images + annotations). We are pursuing the qualification of the final validation dataset as an FDA-qualified medical device development tool [MDDT](https://ncihub.org/groups/httleadership/wiki/HTTPublicWikiMainPage2021622/HTTPublicMedicalDeviceDevelopmentTool2021621) to become a high-value public resource that can be used in AI/ML algorithm submissions and guide others to develop quality validation datasets. 
 * Project overview accepted for publication in the Journal of Pathology Informatics and available [here](https://arxiv.org/abs/2010.06995).

# Why is the FDA Doing This? 
Artificial intelligence (AI) promises to reduce pathologist burden searching and evaluating cells and features on the slides; let the computer do it. AI also promises to help the pathologists be more quantitative and less variable. The regulatory question is then, *“How well can the computer algorithms do the tasks?”* The most practical ground truth for evaluating algorithm performance is pathologist interpretations of the whole slide images. The problem is that pathologist interpretations can vary greatly between other clinicians and their own prior conclusions. Therefore, we need to acknowledge this variability, reduce this variability, and then account for this variability. Tools, methods, and research in this area are lacking, so we are doing it. In this work, we collect data that demonstrates pathologist variability, we create training materials to reduce pathologist variability, and we develop methods to investigate and account for pathologist variability.

# Project Context 
The HTT project is a collaborative project that **crowdsources pathologist annotations.** The annotations we are collecting are estimates of the density of stromal tumor-infiltrating lymphocytes (sTILs) in breast cancer. sTILs are a prognostic biomarker ([Salgado2015_Ann-Oncol_v26p259](https://doi.org/10.1093/annonc/mdu450), [Loi2019_J-Clin-Oncol_v37p559](https://doi.org/10.1200/jco.18.01010)). This project will additionally produce statistical analysis tools to evaluate algorithm performance given the variance in the ground truth. 

# Our Methods 
For our pilot study, we digitized 64 glass slides of stained ductal carcinoma core biopsies prepared at a single clinical site. A collaborating pathologist selected 10 regions of interest (ROIs) per slide for evaluation. We created training materials and workflows to crowdsource pathologist image annotations with two modalities: an optical microscope, **eeDAP**, an Evaluation Environment for Digital and Analog Pathology, and two digital platforms, **caMicroscope,** and **Path Presenter**. (More information in the next section). The annotation workflow asks the pathologist to evaluate the ROI type, make a decision on whether the ROI is appropriate for estimating the density of sTILs, and if appropriate, estimate amount of tumor-associated stroma in the ROI, and estimate the density of sTILs in the stroma. The pilot study data are publicly available [here:](https://github.com/DIDSR/HTT). 

#  Technologies Used in this Project 
### Digital Platforms 
We have two digital platforms for viewing and annotating whole slide images: [PathPresenter](https://htt.pathpresenter.net/) and [caMicroscope](https://wolf.cci.emory.edu/camic/htt/login.html). Pathologists can log in from anywhere in the world and annotate images using these web-based viewers. 

Leadership from Path Presenter and caMicroscope are collaborators on this project and have supported the development of controlled and standardized workflows to select and evaluate ROIs.

### Microscope Platform  
The optical microscope platform uses a hardware and software system called eeDAP, an Evaluation Environment for Digital and Analog Pathology. The eeDAP system registers the live-camera view of the microscope slide with a digital scan of the slide taken with a whole slide imaging system. The eeDAP system is programed to automatically move the motorized stage to pre-specified regions of interest (ROIs) within a slide. Pathologists use the eeDAP software interface to save their evaluations of the ROI. 

The eeDAP system is used to provide the reference standard, eliminating bias from slide digitization. The digital platforms allow us to compare microscope-mode to digital mode evaluations. You can contribute to data collection with the caMicroscope and Path Presenter platforms by completing the  HTT data collection training.

