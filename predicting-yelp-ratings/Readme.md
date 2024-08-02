# Yelp Ratings Predictor

### Original Author
**GitHub Profile**: [Aymen](https://github.com/aymen)

### Original License
**MIT License**  
This project is licensed under the MIT License - see the LICENSE.md file for details.

### Original GitHub Link
[Yelp Ratings Predictor Notebook](https://github.com/aymen/yelp-ratings-predictor)

### Code Adaptation
This project's code was adapted from [Predicting Yelp Ratings](https://github.com/concision/predicting-yelp-ratings), originally developed by concision.

### Description of Project
This project employs natural language processing (NLP) and machine learning in TensorFlow to predict Yelp business ratings from the content of user reviews. By analyzing text data, the model aims to uncover correlations between review sentiments and star ratings, aiding in more accurate business evaluations.

### Required Datasets
**Yelp Open Dataset** - Available on Yelp's dataset page

### How to Download Dataset
To access and download the dataset, please follow these steps:
1. Visit the [Yelp Dataset](https://www.yelp.com/dataset) page.
2. Click on the "Download" button to download the JSON files.
3. Unzip the files into the `data` folder within the project directory, ensuring they are ready for use in the Jupyter notebook.

### Expected Packages and Resource Requirements
**Python Packages**:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- TensorFlow

**Resource Requirements**:
- CPU/GPU

### How To Use
**Setup Environment**:
- Clone the repository or download the specific project files.

**Install Required Packages**:
1. Create and Activate the Virtual Environment:
   - Open your terminal or command prompt within the Jupyter notebook.
   - Navigate to the project directory.
   - Execute commands to create and activate the virtual environment, install ipykernel, and link it to the Jupyter notebook.

2. Install Required Libraries:
   - Activate the virtual environment and install the necessary libraries from the requirements.txt file.

### Additional Library Installation
To enhance the functionality of the CTPO environment, some additional libraries not pre-installed may be required. Follow these steps to install the necessary libraries from the `requirements.txt` file:
1. Open your terminal or command prompt within the Jupyter notebook: `File -> New -> Terminal`.
2. Navigate to the project directory:
   ```bash
   cd /path/to/your/project/directory
   pwd
3. Execute the following commands to create and activate the virtual environment:
   ```bash
   python3 -m venv --system-site-packages myvenv
   source myvenv/bin/activate
   pip3 install ipykernel
   python -m ipykernel install --user --name=myvenv --display-name="Python (myvenv)"
   pip install -r requirements.txt

- After installing libraries from the `requirements.txt` file, ensure you select the correct Python kernel (`Python (myvenv)`) in your Jupyter notebook.

### Run the Notebook:
1. Open the `Yelp_Ratings_Predictor.ipynb` notebook in a Jupyter environment.
2. Execute the notebook cells sequentially to perform data analysis and model training.

### Model Training and Evaluation:
1. Follow the steps within the notebook to train the model using the provided dataset.
2. Evaluate the model's performance and adjust parameters as needed.

### Model Usage:
- Use the trained model to predict Yelp ratings based on new review data, facilitating better business insights and decision-making.

### Troubleshooting
If you encounter issues:
- **Environment Setup**: Ensure that the virtual environment is correctly set up and that all libraries are installed as per the instructions.
- **Dataset Loading**: Verify that the dataset files are correctly placed in the `data` folder and that file paths in the notebook match.

This revised README should now comprehensively cover the setup, usage, and troubleshooting steps for your project. If any more adjustments are needed, please let me know!

