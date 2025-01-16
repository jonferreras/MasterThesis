# Time-Varying Topological Descriptors for Cardiac Disease Diagnosis

## By Jon Ferreras

### Abstract

Cardiac diseases are among the most common illnesses in the world, and data scientists have created a wide range of tools to contribute to their detection and diagnosis. Topological Data Analysis in particular has been used to work for medical imaging and specifically for cardiac MRIs.

This project introduces the use of time-varying topological descriptors along a cardiac cycle and applies them for disease diagnosis. The methods used aim to develop the relationship between TDA and temporal data. We also want to contribute to the simplification, interpretability and improvement of the general approach to cardiac disease diagnosis, which usually involves costly calculations of radiomics or potential black boxes.

### Contents and Procedure

This repository includes the jupyter notebooks used in this thesis. For everything to work correctly, the Automated Cardiac Diagnosis Challenge (ACDC) Dataset should be downloaded without changes from https://humanheart-project.creatis.insa-lyon.fr/database/#collection/637218c173e9f0047faa00fb and the nnunet folder should have the contents described in nnunet/nnUNet_README. 

The image_classification_and_tda notebook extracts the useful images from each patient of the ACDC Dataset, applies two types of segmentation and calculates their topological descriptors, generating several time series that describe each patient's cardiac cycle. This notebook contains a Trial option which allows its running with no more requirements that what is contained in this repository. The Trial folder contains the ACDC data and the nnunet masks from a single patient.

The classification notebook takes the previous time series and extracts features, performs feature selection and uses machine learning models for multi-class classification. The results, including confusion matrices and ROC Curves, are displayed in the notebook. This notebook should be used after a succesful, non-trial run of the image_classification_and_tda notebook.

The visualization notebook contains most images or graphics present in the report. If used, it should be after a succesful, non-trial run of the image_classification_and_tda notebook.


