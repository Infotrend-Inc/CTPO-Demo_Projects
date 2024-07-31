# Fine-tuning TinyBERT for Sentiment Analysis

## Original Author

**GitHub Profile**: [David Chavez](https://github.com/dnachavez)

## Original License

MIT License  
This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/dnachavez/fine-tuning-tinybert-for-sentiment-analysis/blob/main/LICENSE) file for details.

## Original GitHub Link

[Fine-tuning TinyBERT for Sentiment Analysis Notebook](https://github.com/dnachavez/fine-tuning-tinybert-for-sentiment-analysis/blob/main/Fine-tuning%20TinyBERT%20for%20Sentiment%20Analysis.ipynb)

## Description of Project

This project focuses on fine-tuning the TinyBERT model for sentiment analysis. The goal is to leverage the lightweight TinyBERT model to achieve efficient and accurate sentiment classification on a dataset containing text from tweets. By analyzing the sentiment of these tweets, the model can provide valuable insights into public opinion and sentiment trends.

## Required Datasets

Sentiment Analysis Data - [Kaggle Dataset](https://www.kaggle.com/datasets/abhi8923shriv/sentiment-analysis-dataset?select=test.csv)

### How to Download Dataset
To access and download the dataset, please follow these steps:

1. Visit the Kaggle dataset page through the link provided above.
2. Click on the "Download" button on the dataset page to download the dataset zip file.
3. Create a `data` folder in the directory with the Jupyter notebook and unzip the downloaded file into that folder. This step ensures that all data files are ready to be accessed by the notebook.

## Expected Packages and Resource Requirements

**Python Packages**:
- pandas
- numpy
- matplotlib
- scikit-learn
- transformers
- torch
- nltk

**Resource Requirements**:
- CPU or GPU (optional for faster training)

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
   
   Before running the following command in jupyter notebook, make sure you are in the directory where the Jupyter Notebook and virtual environment is located. This ensures the ./ path is always current. You can use the cd command to change to your project directory and pwd to verify your current directory.
   
   ```
   !. ./myvenv/bin/activate; pip install -r requirements.txt
   ```

3. **Run the Notebook**:
   - Open the `Fine_tuning_TinyBERT_for_Sentiment_Analysis.ipynb` notebook in a Jupyter environment.
   - Execute the notebook cells sequentially to perform data analysis, model training, and evaluation.

4. **Model Training and Evaluation**:
   - Follow the steps within the notebook to train the model using the provided dataset.
   - Evaluate the model's performance and tweak parameters as necessary to improve accuracy.

5. **Model Usage**:
   - The trained model can be used to predict the sentiment of new text data, providing insights into public opinion and sentiment trends.

## Troubleshooting

- Ensure that the name of the dataset file is the same as referenced in the notebook.
- Make sure the Jupyter notebook and the dataset are in the same folder to avoid file path issues.
- Change the model saving path based on your directory structure to ensure the model is saved correctly.

## Changes Made to the Original Notebook

- Performed Exploratory Data Analysis (EDA) to understand the dataset.
- Changed the dataset path from the original notebook, which used a drive, to a local dataset.
- Updated the `load_dataset` function to ensure it runs properly with the new dataset.

