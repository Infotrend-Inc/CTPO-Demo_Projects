# OpenVoice: Advanced Voice Cloning and Synthesis

## Project Overview

OpenVoice is a cutting-edge project dedicated to the development of voice cloning and speech synthesis technologies. This repository hosts the tools and models necessary for implementing state-of-the-art voice cloning capabilities, enabling users to create lifelike synthetic voices from audio samples.

## Original GitHub Link

[OpenVoice Project Repository](https://github.com/myshell-ai/OpenVoice)


## Voice Translation Widgets

This application provides a user-friendly interface for voice translation. Below are the features available:

### Features

1. **Voice Upload**: Users can upload their voice recordings in MP3 format.
   
2. **Language Selection**: A dropdown menu allows users to select the language of the text to which the uploaded voice will be translated.
   
3. **Text Input Box**: Users can input or edit the text that will be translated into the selected language using the uploaded voice.

### Usage

- **Uploading Voice**: Click on the 'Upload' button and select an MP3 file from your device.
- **Selecting Language**: Use the dropdown to choose the target language for translation.
- **Entering Text**: Type into the text box the text you want to use for translation.

This application is designed to be intuitive and easy to use, ensuring that users can quickly translate voices with minimal effort.

## System Requirements

- **Python 3.x**: Ensure Python 3.x is installed.
- **Operating System**: Linux or macOS (for complete compatibility with all tools and scripts).

## Setup and Installation

## How To Use

1. **Setup Environment**:
   - Clone the repository or download the specific project files.
   - Ensure Python 3.x is installed.

2. **Install Required Packages**:

   - To enhance the functionality of the CTPO environment, you may need to install some libraries not pre-installed but required for this notebook. Follow these steps to install the necessary libraries from the `requirements.txt` file:

   **2.1 Create and Activate the Virtual Environment:**
   
   Open your terminal or command prompt within the jupyter notebook. `File -> New -> Terminal`
   
   Navigate to the project directory where you want to set up the environment.
   
   Execute the following commands to create and activate the virtual environment:
   
   ```
   bash
   python3 -m venv --system-site-packages myvenv #myvenv is name of virtual environment you can change it
   source myvenv/bin/activate
   pip3 install ipykernel
   python -m ipykernel install --user --name=myvenv --display-name="Python (myvenv)"
   ```

 **2.2 Install Required Libraries**
   
 Before running the following command in the Jupyter notebook, make sure you are in the directory where the Jupyter Notebook and virtual environment is located. Load the newly created "Python (myvenv)" kernel. This ensures the `./` path is always current. You can use the `cd` command to change to your project directory and `pwd` to verify your current directory.

   ```sh
   !. ./myvenv/bin/activate; pip install -r requirements.txt
   ```

## Model Preparation
Download and prepare the model data:

1. Create a directory for model checkpoints:
   ```
   mkdir checkpoints_v2
    ```
2. Download the model checkpoint data:
   ```
   wget https://myshell-public-repo-host.s3.amazonaws.com/openvoice/checkpoints_v2_0417.zip
    unzip checkpoints_v2_0417.zip -d checkpoints_v2
    ```
   
## Run the Notebook:
- Open the `demo.ipynb` notebook in a Jupyter environment.
-  Follow the instructions within the notebook, executing the code cells in sequence. Each cell includes comments explaining the purpose of the code, which will guide you through the demo process.
- Make sure to read any embedded instructions or comments carefully to maximize your understanding and troubleshooting any issues that may arise.

## Troubleshooting
### Common Issues and Fixes
CUDA Library Error: If you encounter an error related to libcublas.so.11, create a symbolic link to the newer version:
    ```
    ln -s /usr/local/cuda/lib64/libcublas.so.12 /usr/local/cuda/lib64/libcublas.so.11
    ```
Install portaudio: Portaudio is required for handling audio input and output in many applications. If you experience issues related to audio operations, ensure that `portaudio19-dev` is installed:
    ```
    ! apt install -y portaudio19-dev
    ```
This ensures that all dependencies for audio processing are properly configured.