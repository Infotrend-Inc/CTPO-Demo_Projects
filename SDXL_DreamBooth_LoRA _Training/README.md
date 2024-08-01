# SDXL DreamBooth LoRA Training

## Original Author

**GitHub Profile**: [Hugging Face](https://github.com/huggingface)

## Original License

MIT License  
This project is licensed under the MIT License - see the [LICENSE](https://github.com/huggingface/notebooks/blob/main/LICENSE) file for details.

## Original Jupyter Notebook

[SDXL DreamBooth LoRA Training Notebook](https://github.com/huggingface/notebooks/blob/main/diffusers/SDXL_DreamBooth_LoRA_.ipynb)

## Description of Project

This project demonstrates the training of a Stable Diffusion model using the DreamBooth technique with Low-Rank Adaptation (LoRA). The goal is to fine-tune a pre-trained diffusion model on a custom dataset of images, enhancing its ability to generate specific content based on the provided training images.

In this instance, the model is trained on a dataset of 10 images featuring the cartoon character Tom from "Tom and Jerry". The trained model can then be used to generate images that closely resemble the style and features of the character.

## Dataset

The dataset used for this project consists of 10 images of the cartoon character Tom from "Tom and Jerry". You can train the model on any dataset of your choice by providing the appropriate images.

### Dataset Details

- **Source**: Custom dataset created from images of Tom.
- **Number of Images**: 10
- **Image Type**: Cartoon character images

## How To Use

1. **Setup Environment**:
   - Clone the repository or download the specific project files.
   - Ensure Python 3.x is installed.
   - Install the required packages listed in the `requirements.txt` file.

2. **Install Required Packages**:
   
   - To enhance the functionality of the CTPO environment, you may need to install some libraries not pre-installed but required for this notebook. Follow these steps to install the necessary libraries:

   **2.1 Create and Activate the Virtual Environment:**
   
   Open your terminal or command prompt within the Jupyter notebook. Navigate to `File -> New -> Terminal` and type `bash` to get a shell compatible with the following commands.

   Navigate to the project directory where you want to set up the environment.

   Execute the following commands to create and activate the virtual environment:

   ```sh
   bash
   python3 -m venv --system-site-packages myvenv
   source myvenv/bin/activate
   pip3 install ipykernel
   python -m ipykernel install --user --name=myvenv --display-name="Python (myvenv)"
   ```

   **2.2 Install Required Libraries**

   Before running the following command in the Jupyter notebook, make sure you are in the directory where the Jupyter Notebook and virtual environment is located. Load the newly created "Python (myvenv)" kernel. This ensures the `./` path is always current. You can use the `cd` command to change to your project directory and `pwd` to verify your current directory.

   ```sh
   !. ./myvenv/bin/activate; pip install -r requirements.txt
   ```

3. **Run the Notebook**:
   - Open the `PHOTO_TRAINING.ipynb` notebook in a Jupyter environment.
   - Load the "Python (myvenv)" kernel.
   - Execute the notebook cells sequentially to perform data loading, preprocessing, model training, and evaluation.

4. **Model Training and Evaluation**:
   - Follow the steps within the notebook to train the model using the provided dataset.

5. **Model Usage**:
   - The trained model can be used to generate new images that resemble the cartoon character Tom. You can adapt the notebook to use different datasets and generate images based on the specific content of your choice.

## Ensure Proper Folder Structure

Make sure that the folders in your directory are structured as follows to ensure the notebook runs correctly:
- The dataset images should be placed in the appropriate directory as specified in the notebook.
- Ensure any output directories specified in the notebook exist or adjust the paths accordingly.

## Changes Made to the Original Notebook

1. **Dataset Adaptation**:
   - Changed the dataset to focus on the cartoon character Tom from "Tom and Jerry".

2. **User Image Upload**:
   - Added functionality to allow users to upload images directly within the notebook. The uploaded images are stored in a designated directory and used for model training.

3. **Efficiency Improvements**:
   - Modified the notebook to enhance efficiency by reducing redundant loading operations.
