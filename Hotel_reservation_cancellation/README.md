# Hotel Reservations Cancellation Prediction

## Original Author

**GitHub Profile**: [Sukhman Singh](https://github.com/SUKHMAN-SINGH-1612)

## Original License

MIT License  
This project is licensed under the MIT License - see the [LICENSE](https://github.com/SUKHMAN-SINGH-1612/Data-Science-Projects/blob/main/LICENSE) file for details.

## Original Notebook

[Hotel Reservations Cancellation Prediction Notebook](https://github.com/SUKHMAN-SINGH-1612/Data-Science-Projects/blob/main/Hotel%20Reservations%20Cancellation%20Prediction/Hotel%20Reservations%20Cancelation%20Prediction.ipynb)

## Description of Project

This project focuses on predicting hotel reservation cancellations by analyzing various features associated with reservations. By using machine learning techniques, the model aims to identify patterns and factors that contribute to cancellations, enabling hotels to take proactive measures to reduce cancellation rates and optimize revenue management.

## Required Datasets

Hotel Reservations Data - [Kaggle Dataset](https://www.kaggle.com/datasets/ahsan81/hotel-reservations-classification-dataset)

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
   - Open the `Hotel_reservation_cancellation.ipynb` notebook in a Jupyter environment.
   - Execute the notebook cells sequentially to perform data analysis, model training, and evaluation.

4. **Model Training and Evaluation**:
   - Follow the steps within the notebook to train the model using the provided dataset.
   - Evaluate the model's performance and tweak parameters as necessary to improve accuracy.

5. **Model Usage**:
   - The trained model can be used to predict cancellations for new reservations, helping hotels to better manage their bookings and reduce revenue loss.


