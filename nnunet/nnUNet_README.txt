These are the steps to follow to generate the masks for the 150 patients / 1600+ frames. Change every path for your own.

First, create folders called "raw", "pre", "models" and "output" inside of this current "nnunet" folder and run this in the terminal:

set nnUNet_raw=C:\Users\jonfe\Documents\MasterThesis\nnunet\raw
set nnUNet_preprocessed=C:\Users\jonfe\Documents\MasterThesis\nnunet\pre
set nnUNet_results=C:\Users\jonfe\Documents\MasterThesis\nnunet\models

Then, the "models" folder should contain the segmentation model inside of a folder called "Dataset_ACDC". 
The model that we used is not public and it belongs to the BCN-AIM Lab, so we can't provide it here (also because it is 3GB+ heavy). 
The raw and pre folders can remain empty.

Finally, after having generated the "3DImagesPreFilter" folder in the "image_processing_and_tda" notebook,  run this in the terminal.
The "cpu" can be changed to "gpu" or "cuda".

nnUNetv2_predict -i C:\Users\jonfe\Documents\MasterThesis\3DImagesPreFilter -o C:\Users\jonfe\Documents\MasterThesis\nnunet\output -d "Dataset_ACDC" -c 3d_fullres --save_probabilities -device cpu

