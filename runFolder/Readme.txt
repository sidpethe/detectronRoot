-------------------------------------------------------------------------
-------------------------------------------------------------------------
Author: Siddharth Pethe

Description: This file contains information on Folder structure for output Directory named runFolder.

-------------------------------------------------------------------------
-------------------------------------------------------------------------

Root Directory: runFolder

    centroids.txt: This file is created to hold the centroid of every detected object. 
                   Column 1: Input File Name
                   Column 2: Object Class
                   Column 3: Centroid X
                   Column 4: Centroid Y
                   
                 
    Readme.txt   : Current File
        
runFolder -> kitti_results:
    This subdirectory contains the output images and folder structure as required by Kitti evaluation script.

runFolder -> kitti_results -> pred_list:
    This folder contains text files for every input image. 
    
    Every file has single row for every detected object in the format:-
        Column 1: Relative path to mask file
        Column 2: Class Label ID according to Cityscapes/KITTI labels.py file
        Column 3: Confidence of detection
    
runFolder -> kitti_results -> pred_img:
    This folder contains the detected object masks as referenced in "pred_list".
    
