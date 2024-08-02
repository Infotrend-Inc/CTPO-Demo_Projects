# Project: Fashion MNIST Classification using Neural Networks

## Original Author
- Sunil Singh
- [GitHub Profile](https://github.com/sssingh)

## Original License
- [MIT License](https://choosealicense.com/licenses/mit/)
- This project is licensed under the MIT License - see the LICENSE.md file for details.

## Original GitHub Link
- [Fashion MNIST Classification Repository](https://github.com/sssingh/fashion-mnist-classification)

## Description of Project
This project utilizes a custom-built, fully-connected neural network to classify apparel images from the Fashion-MNIST dataset. Developed as a more complex alternative to the standard MNIST digit classification, this project serves as a benchmark for neural network capabilities in multi-label image classification.

## Required Datasets
- Fashion MNIST dataset (included in PyTorch's torchvision package)
- [Direct dataset links](https://www.tensorflow.org/tutorials/keras/classification)

## Resource Requirements
- CPU or GPU (NVIDIA GPU recommended for optimal performance)
- Recommended GPU: NVIDIA Quadro P5000 with 16GB memory
- Approximate training and validation time for 35 epochs: 15 minutes on recommended GPU setup.

## Capabilities to Run on CPU and/or GPU
This project is configured to automatically detect and utilize a GPU if available, ensuring faster processing and training times. If a GPU is not available, the project will gracefully fallback to using the CPU.

## How To Use
To get started with this project, follow these steps:

1. **Setup Environment:**
   - Clone the repository or download all project files, including the `Fashion_MNIST_Classification.ipynb` notebook.
   - No installation of packages is required as the project runs within the Infotrend pre-built container which includes all necessary dependencies.

2. **Run the Notebook:**
   - Open the `Fashion_MNIST_Classification.ipynb` notebook using Jupyter Notebook or JupyterLab.
   - Execute the notebook cells sequentially from start to finish. The environment will automatically detect and utilize a GPU if available; otherwise, it will use the CPU.

3. **Model Training and Evaluation:**
   - Follow the steps in the notebook to train and evaluate the neural network model on the Fashion MNIST dataset.
   - The notebook provides detailed instructions and visualizations of the training process and model performance.

4. **Model Usage:**
   - Once trained, the model can classify new images of apparel from the Fashion MNIST dataset. Instructions for using the model for prediction are provided within the notebook.

## Troubleshooting Guides
This section addresses common issues you might encounter when running the `Fashion_MNIST_Classification.ipynb` notebook:

### Issue 1: Environment Setup Failures
**Symptom:** Failure to launch the Jupyter Notebook in the Infotrend container.
**Solution:** Ensure the Infotrend container is running and properly set up. Verify network settings and container configurations. Restart the container if necessary.

### Issue 2: Model Not Training
**Symptom:** The model does not show improvement over epochs.
**Solution:** Check the learning rate and optimizer settings. Ensure that the dataset is correctly loaded and preprocessed. Consider modifying hyperparameters or increasing the dataset size for training.

### Issue 3: GPU Utilization Not Detected
**Symptom:** The system falls back to CPU even though a GPU is available.
**Solution:** Verify the GPU installation and driver updates. Ensure PyTorch is configured to recognize the GPU. Use the command `torch.cuda.is_available()` to check GPU availability from within the notebook.

### Algorithm Insights
The fully-connected neural network used in this project is designed for simplicity to demonstrate basic image classification techniques. While it lacks the spatial hierarchy of convolutional networks, it serves as a practical starting point for understanding neural network operations. For more complex image recognition tasks, consider exploring architectures involving convolutional layers that preserve spatial relationships within images.

[Back to Top](#project-fashion-mnist-classification-using-neural-networks)
