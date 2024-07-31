# Sleep Disorder Prediction

## Original Author

**GitHub Profile**: [Sukhman Singh](https://github.com/SUKHMAN-SINGH-1612)

## Original License

MIT License  
This project is licensed under the MIT License - see the [LICENSE](https://github.com/SUKHMAN-SINGH-1612/Data-Science-Projects/blob/main/LICENSE) file for details.

## Original Notebook

[Sleep Disorder Prediction Notebook](https://github.com/SUKHMAN-SINGH-1612/Data-Science-Projects/blob/main/Sleep%20Disorder%20Prediction/Sleep%20Disorder%20Prediction.ipynb)

## Description of Project

This project focuses on predicting sleep disorders by analyzing various lifestyle and medical variables such as age, BMI, physical activity, sleep duration, blood pressure, and more. By utilizing machine learning techniques, the model aims to identify patterns and factors contributing to sleep disorders, enabling early intervention and improved healthcare outcomes.

## Required Datasets

**Sleep Health and Lifestyle Dataset** - [Kaggle Dataset](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset)

### How to Download Dataset

To access and download the dataset, please follow these steps:

1. Visit the Kaggle dataset page through the link provided above.
2. Click on the "Download" button on the dataset page to download the dataset zip file.
3. Unzip the downloaded file into the folder where you will run the Jupyter notebook. This step ensures that all data files are ready to be accessed by the notebook.

## Expected Packages and Resource Requirements

**Python Packages**:
- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn

**Resource Requirements**:
- CPU

## How To Use

1. **Setup Environment**:
   - Clone the repository or download the specific project files.
   - Ensure Python 3.x is installed.

2. **Install Required Packages**:

   To enhance the functionality of the CTPO environment, you may need to install some libraries not pre-installed but required for this notebook. Follow these steps to install the necessary libraries from the `requirements.txt` file:

   **2.1 Create and Activate the Virtual Environment:**
   
   Open your terminal or command prompt within the Jupyter notebook. `File -> New -> Terminal`

   Navigate to the project directory where you want to set up the environment.

   Execute the following commands to create and activate the virtual environment:

   ```sh
   bash
   python3 -m venv --system-site-packages myvenv #myvenv is name of virtual environment you can change it
   source myvenv/bin/activate
   pip3 install ipykernel
   python -m ipykernel install --user --name=myvenv --display-name="Python (myvenv)"
   ```

   **2.2 Install Required Libraries**

   Before running the following command in the Jupyter notebook, make sure you are in the directory where the Jupyter Notebook and virtual environment is located. This ensures the `./` path is always current. You can use the `cd` command to change to your project directory and `pwd` to verify your current directory.

   ```sh
   !. ./myvenv/bin/activate; pip install -r requirements.txt
   ```

3. **Run the Notebook**:
   - Open the `Sleep_Disorder_Prediction.ipynb` notebook in a Jupyter environment.
   - Load the "Python (myvenv)" kernel.
   - Execute the notebook cells sequentially to perform data analysis, model training, and evaluation.

4. **Model Training and Evaluation**:
   - Follow the steps within the notebook to train the model using the provided dataset.
   - Evaluate the model's performance and tweak parameters as necessary to improve accuracy.

5. **Model Usage**:
   - The trained model can be used to predict sleep disorders for new data, helping healthcare professionals to identify at-risk individuals and provide early interventions.

## Ensure Proper Folder Structure

Make sure that the folders in your directory are structured as follows to ensure the notebook runs correctly:
- The dataset file `Sleep_health_and_lifestyle_dataset.csv` should be in the same directory as the notebook.
- Ensure any output directories specified in the notebook exist or adjust the paths accordingly.
