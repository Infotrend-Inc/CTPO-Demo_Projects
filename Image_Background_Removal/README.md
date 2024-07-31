# Image Background Removal

## Original Author

**GitHub Profile**: [Shreyas BK](https://github.com/shreyas-bk)

## Original License

MIT License  
This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/shreyas-bk/u2netdemo/blob/master/LICENSE) file for details.

## Original GitHub Link

[Image Background Removal Notebook](https://github.com/shreyas-bk/u2netdemo/blob/master/DEMOS/U_2_Netp_Demonstration_Colab.ipynb)

## Description of Project

This project demonstrates the use of U-2-NETp for various image processing tasks, including background removal, bounding box creation, and salient feature highlighting. U-2-NETp is a lightweight model designed for salient object detection.

## Changes Made to the Original Notebook

- Removed the need to clone other repositories by adjusting the paths within both the notebook and the `u2net_test.py` script.

- Created a function in the notebook that allows users to upload images, which are then stored in the images folder.

- Adjusted the `u2net_test.py` script to process the uploaded images and store the results in the results folder.

- The notebook uses the results from the `u2net_test.py` script to remove backgrounds, create bounding boxes, and highlight salient features in the images.

## Required Datasets

No external datasets are required for this demonstration as it utilizes user-uploaded images.

## Expected Packages and Resource Requirements

**Python Packages**:
- numpy
- tensorflow
- pillow
- opencv-python
- os
- pytorch
- glob

**Resource Requirements**:
- CPU or GPU (optional for faster processing)

### Run the Notebook:

1. Open the `Image_Removal.ipynb` notebook in a Jupyter environment.
2. Execute the notebook cells sequentially to see desire results.


### Model Usage:

The trained model can be used to:
- Remove backgrounds from images.
- Create bounding boxes around objects.
- Highlight salient features in images.

### Ensure Proper Folder Structure

Make sure you have the folders set up the same way as in the repository to ensure the notebook runs correctly. Specifically, ensure that the `images` and `results` directories are created in the project root directory as shown in the setup steps.
