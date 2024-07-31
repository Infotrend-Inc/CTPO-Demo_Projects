# Next Word Prediction

## Original Author

**GitHub Profile**: [Susanta Biswas](https://github.com/susantabiswas)

## Original License

MIT License  
This project is licensed under the MIT License - see the [LICENSE](https://github.com/susantabiswas/Word-Prediction-Ngram/blob/master/LICENSE) file for details.

## Original Notebook

[Next Word Prediction Notebook](https://github.com/susantabiswas/Word-Prediction-Ngram/blob/master/Word_Prediction_GoodTuring_Smoothing_with_Interpolation.ipynb)

## Introduction and Objective

In the era of advanced natural language processing, predictive text systems have become an integral part of user interfaces, enhancing user experience by providing suggestions and auto-completing text inputs. This notebook demonstrates the implementation of a next word prediction system using an N-gram model with Good-Turing smoothing and interpolation techniques. An N-gram model is a type of probabilistic language model that predicts the next item in a sequence based on the previous items, making it a powerful tool for understanding and generating human language.

The primary objective of this project is to build a robust word prediction system by leveraging statistical language modeling techniques. The N-gram model is trained on a large corpus of text data, allowing it to learn the probabilities of sequences of words. To address the issue of zero probabilities for unseen N-grams, Good-Turing smoothing is applied, which adjusts the probability estimates for rare or unseen events. Additionally, interpolation combines the probabilities of different N-grams (e.g., bigrams, trigrams) to improve prediction accuracy. This combination of techniques ensures that the model can make accurate and reliable predictions, even when encountering new or uncommon word sequences.

## Dataset

The dataset used for training and evaluating the N-gram model is included in this repository. Specifically, the following files are used:
- `internet_archive_scifi_v3.txt`: This file is used for training the N-gram model. It contains a large corpus of science fiction text data from which the model learns the probabilities of word sequences.

You can find the dataset at this [Kaggle link](https://www.kaggle.com/datasets/jannesklaas/scifi-stories-text-corpus).

This science fiction dataset will be utilized to complete sentences and generate text relevant to the genre, ensuring the model can capture the unique vocabulary and stylistic elements typical of science fiction narratives.

## Installing Libraries

To enhance the functionality of the environment, you may need to install some libraries not pre-installed in the CTPO environment but required for this notebook. Follow these steps to install the necessary libraries from the `requirements.txt` file:

### 1. Create and Activate the Virtual Environment

Open your terminal or command prompt within the Jupyter notebook. Navigate to `File -> New -> Terminal` and type `bash` to get a shell compatible with the following commands.

Navigate to the project directory where the notebook is to set up the environment.

Execute the following commands to create and activate the virtual environment:

```sh
bash
python3 -m venv --system-site-packages myvenv
source myvenv/bin/activate
pip3 install ipykernel
python -m ipykernel install --user --name=myvenv --display-name="Python (myvenv)"
```

### 2. Install Required Libraries

Before running the following command in the Jupyter notebook, make sure you are in the directory where the Jupyter Notebook and virtual environment is located. Load the newly created "Python (myvenv)" kernel. This ensures the `./` path is always current. You can use the `cd` command to change to your project directory and `pwd` to verify your current directory.

```sh
!. ./myvenv/bin/activate; pip install -r requirements.txt
```

### Important Note

It is crucial to load the new "myvenv" kernel for the notebook to work correctly. If the new "myvenv" kernel is not loaded, the required libraries and environment settings will not be applied, and the notebook will not function as expected.

## Running the Notebook

1. **Setup Environment**:
   - Clone the repository or download the specific project files.
   - Ensure Python 3.x is installed.

2. **Run the Notebook**:
   - Open the `Next_Word_Prediction.ipynb` notebook in a Jupyter environment.
   - Load the "Python (myvenv)" kernel.
   - Execute the notebook cells sequentially to perform data analysis, model training, and evaluation.

3. **Model Training and Evaluation**:
   - Follow the steps within the notebook to train the model using the provided dataset.
   - Evaluate the model's performance and tweak parameters as necessary to improve accuracy.

4. **Model Usage**:
   - The trained model can be used to predict the next word in a sequence, helping to complete sentences and generate coherent text relevant to the science fiction genre.

## Changes Made to the Original Notebook

1. **Dataset Update**:
   - The original dataset was replaced with a dataset focused on science fiction stories to better capture the vocabulary and style of the genre.
2. **Function Updates**:
   - The `doPredictionBackoffGT` function was modified to consider the entire sentence rather than just the last three elements.
   - The `takeInput` function was also adjusted to accommodate the changes in `doPredictionBackoffGT`.
3. **Performance Improvement**:
   - Introduced the `dictss` function to load the training file once and generate the necessary dictionaries. This change prevents the need to reload the entire corpus each time the `word_prediction` function is called, improving efficiency.

## Ensure Proper Folder Structure

Make sure that the folders in your directory are structured as follows to ensure the notebook runs correctly:
- The dataset file should be in the same directory as the notebook.
