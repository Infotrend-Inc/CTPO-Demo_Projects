# Natural Language Processing with Disaster Tweets

## Original Author

**GitHub Profile**: [Sugata Ghosh](https://github.com/sugatagh)

## Original License

MIT License  
This project is licensed under the MIT License - see the LICENSE file for details in the original repository.

## Original GitHub Link

[Natural Language Processing with Disaster Tweets Notebook](https://github.com/sugatagh/Natural-Language-Processing-with-Disaster-Tweets)

## Description of Project

This project uses natural language processing techniques to analyze tweet data and classify tweets as related to real-world disasters or not. The aim is to automate the detection of disaster-related communications, which are crucial during emergency response situations.

## Required Datasets

**Disaster Tweets Dataset**:

This project utilizes two primary datasets, `train.csv` and `test.csv`, which should be downloaded and stored in a `data` directory accessible by the notebook.

### How to Download Dataset
To access and set up the datasets, please follow these steps:

1. Create a `data` folder in your project directory if it doesn't already exist.
2. Download the `train.csv` and `test.csv` files from the following Kaggle competition link:
   - [Natural Language Processing with Disaster Tweets](https://www.kaggle.com/c/nlp-getting-started/data) (those datasets have special rules as can be seen at [https://www.kaggle.com/c/nlp-getting-started/rules](https://www.kaggle.com/c/nlp-getting-started/rules))
3. Place the downloaded `train.csv` and `test.csv` files into the `data` folder. This step ensures that all data files are ready to be accessed by the notebook.

### Additional JSON Resources
Alongside the main datasets, the project utilizes two JSON files for text preprocessing. Ensure these files are also placed in the `data` directory:
- **`english_contractions_lowercase.json`**: Contains mappings for English contractions to their expanded forms, crucial for normalizing the text data.
- **`english_acronyms_lowercase.json`**: Provides mappings for common English acronyms to their full forms, assisting in clarifying the text content.

### File Descriptions
- **train.csv**: Contains the tweets and labels for training your model. Each row in this file corresponds to a tweet, and includes the text of the tweet along with a binary label indicating whether the tweet is about a real disaster (1) or not (0).
- **test.csv**: Contains the tweets for which you will predict the disaster relevance. This file includes only the text of the tweets without any labels.

### Setup for Dataset Use
After placing the files in the `data` directory, ensure your Jupyter notebook is configured to read from this directory. This might involve setting the correct path to the `data` folder in your data loading script or notebook cells.


## Contents of the Notebook

- **Introduction**: Overview of the project's aim and importance.
- **Basic Exploratory Data Analysis**: Initial analysis of the data to understand the distribution and nature of the dataset.
- **Text Normalization**: Processing steps to clean and normalize the text data.
- **Bag of N-grams Model**: Implementation of a Bag of N-grams model to predict disaster relevance.
- **TF-IDF Model**: Utilization of TF-IDF scores for feature extraction and model training.
- **Acknowledgements**: Credits to data providers and contributors.
- **References**: Sources and inspirations for the project methodology.

## Expected Packages and Resource Requirements

**Python Packages**:
- numpy
- pandas
- scikit-learn
- nltk
- xgboost
- seaborn
- wordcloud

**Resource Requirements**:
- CPU or GPU (GPU recommended for faster processing)

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
### Important Note

It is crucial to load the new "myvenv" kernel for the notebook to work correctly. If the new "myvenv" kernel is not loaded, the required libraries and environment settings will not be applied, and the notebook will not function as expected.

3. **Run the Notebook**:
    Open the natural-language-processing-with-disaster-tweets.ipynb notebook in a Jupyter environment.
    Execute the notebook cells sequentially to perform data loading, preprocessing, model training, and evaluation.
   
5. **Model Usage**:
- **Predictive Capability**: The trained model can accurately determine whether a tweet is related to an actual disaster. This capability is crucial for enabling rapid response and effective communication during emergency situations.
