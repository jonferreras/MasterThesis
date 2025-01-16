# Time-Varying Topological Descriptors for Cardiac Disease Diagnosis

## By Jon Ferreras

### Abstract

Cardiac diseases are among the most common illnesses in the world, and data scientists have created a wide range of tools to contribute to their detection and diagnosis. Topological Data Analysis in particular has been used to work for medical imaging and specifically for cardiac MRIs.

This project introduces the use of time-varying topological descriptors along a cardiac cycle and applies them for disease diagnosis. The methods used aim to develop the relationship between TDA and temporal data. We also want to contribute to the simplification, interpretability and improvement of the general approach to cardiac disease diagnosis, which usually involves costly calculations of radiomics or potential black boxes.

### Contents

This repository includes the jupyter notebooks used in this thesis.

The image_classification_and_tda notebook performs the segmentation 

For this code to work properly, the ACDC Dataset should be downloaded without changes from https://humanheart-project.creatis.insa-lyon.fr/database/#collection/637218c173e9f0047faa00fb and an nnunet folder with the model used for segmentation in the same directory as this notebook. In the Github repository (https://github.com/jonferreras/MasterThesis) there is trial data (just one patient and its segmentation masks) that allows testing of this notebook. The next flag controls the use of either option (False means default use, True means Trial use)
