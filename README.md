# FDG-PET/CT_AI
This repository is created to release the model weights for the following paper: "Development and validation of pan-cancer lesion segmentation AI-model for whole-body 18F-FDG PET/CT in diverse clinical cohorts"



We have used 3D full resolution nnUNet model( https://www.nature.com/articles/s41592-020-01008-z) and the model was developed using the same instruction as by the nnUNet repository (https://github.com/MIC-DKFZ/nnUNet). 
1. First, create a Python environment. You can name it to your liking; for example, 'petct-env'.
        'petct-env' -m venv moose-env
2. Install nnUNet. Installation process can be found in the following link: [documentation/installation_instructions.md](https://github.com/MIC-DKFZ/nnUNet/blob/master/documentation/installation_instructions.md)
3. Create a new folder (anyname). Create the following three sub-folder in this directory: 'nnUNet_raw', 'nnUNet_preprocessed','nnUNet_results' inside the folder. The names should be exactly the same.
4. Create another folder "Dataset101_PETCT" inside 'nnUNet_raw', 'nnUNet_preprocessed','nnUNet_results' folders. This is important for nnUNet to identify which dataset to process.
5. The image files needs to be put inside the '/nnUNet_raw/Dataset101_PETCT' path.
6. put the following files inside '/nnUNet_preprocessed/Dataset101_PETCT' path.
   
   
7. nnU-Net expects datasets in a structured format. This format is inspired by the data structure of the Medical Segmentation Decthlon. Please read the following link for dataset conversion: https://github.com/MIC-DKFZ/nnUNet/blob/master/documentation/how_to_use_nnunet.md
8. For model development: AUTOPET open access dataset has been used. The dataset can be downloaded from https://drive.google.com/drive/folders/1luNhXZtdn2d12nPmLOMWTAjNCiqQOu4u?usp=drive_link
9. Model weights can be downloaded from google drive: https://drive.google.com/drive/folders/1luNhXZtdn2d12nPmLOMWTAjNCiqQOu4u?usp=sharing
10. Use inference.sh to run inference using the model weights. The folders and data structure as same as instructed for nnUNet. 
