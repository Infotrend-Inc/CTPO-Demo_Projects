# CTPO: Tech Projects

Examples using CTPO (CUDA, TensorFlow, PyTorch, OpenCV) as their source container.

CTPO: https://github.com/Infotrend-Inc/CTPO

CTPO (CUDA, TensorFlow, PyTorch, OpenCV) is a powerful environment designed to facilitate machine learning, computer vision and NLP projects. These examples have been adapted from public sources and presented as Jupyter Notebooks to demonstrate the versatility and capabilities of CTPO. Each project leverages different libraries and tools within the CTPO environment to solve domain-specific problems. This collection serves as a practical resource for developers and researchers to explore various machine learning, computer vision and NLP techniques.


## Project List

| Domain | Project Name | Link to Directory |
| --- | --- | --- |
| Computer Vision | Fashion MNIST Classification | [Fashion_MNIST_Classification](https://github.com/Infotrend-Inc/CTPO-Demo_Projects/tree/main/Fashion_MNIST_Classification) |
| Computer Vision | Fast Neural Style Transfer | [Fast_neural-Style-Transfer](https://github.com/Infotrend-Inc/CTPO-Demo_Projects/tree/main/Fast_neural-Style-Transfer) |
| Computer Vision | Image Background Removal | [Image_Background_Removal](https://github.com/Infotrend-Inc/CTPO-Tech_Projects/tree/main/Image_Background_Removal) |
| Data Science | Amex Default Prediction | [amex-default-prediction](https://github.com/Infotrend-Inc/CTPO-Demo_Projects/tree/main/amex-default-prediction) |
| Data Science | Home Credit Default Risk Recognition | [Home-Credit-Default-Risk-Recognition](https://github.com/Infotrend-Inc/CTPO-Demo_Projects/tree/main/Home-Credit-Default-Risk-Recognition) |
| Data Science | Hotel reservation cancellation Prediction | [Hotel_reservation_cancellation](https://github.com/Infotrend-Inc/CTPO-Tech_Projects/tree/main/Hotel_reservation_cancellation) |
| Data Science | Predicting Yelp Ratings | [predicting-yelp-ratings](https://github.com/Infotrend-Inc/CTPO-Demo_Projects/tree/main/predicting-yelp-ratings) |  
| Data Science | Wind turbine failure detection | [Wind_turbine_failure_detection](https://github.com/Infotrend-Inc/CTPO-Tech_Projects/tree/main/Wind_turbine_failure_detection) |
| Machine Learning | Electrical Transmission lines Fault detection | [Electrical_Fault_Detection_Classification](https://github.com/Infotrend-Inc/CTPO-Tech_Projects/tree/main/Electrical_Fault_Detection_Classification) |
| Machine Learning| SDXL DreamBooth LoRA Training | [SDXL_DreamBooth_LoRA_Training](https://github.com/Infotrend-Inc/CTPO-Demo_Projects/tree/main/SDXL_DreamBooth_LoRA%20_Training) |
| Machine Learning | Sleep Disorder Prediction | [Sleep_Disorder_prediction](https://github.com/Infotrend-Inc/CTPO-Tech_Projects/tree/main/Sleep_Disorder_prediction) |
| Natural Language Processing | Next Word Prediction | [Next_word_prediction](https://github.com/Infotrend-Inc/CTPO-Tech_Projects/tree/main/Next_word_prediction) |
| Natural Language Processing | NLP with Disaster Tweets | [NLP_with_DisasterTweets](https://github.com/Infotrend-Inc/CTPO-Demo_Projects/tree/main/NLP_with_DisasterTweets) |
| Natural Language Processing | Sentiment Analysis | [Sentiment_Analysis](https://github.com/Infotrend-Inc/CTPO-Tech_Projects/tree/main/Sentiment_Analysis) |
| Natural Language Processing | Open Voice Clone | [OpenVoiceClone](https://github.com/Infotrend-Inc/CTPO-Demo_Projects/tree/main/OpenVoiceClone) |
| Natural Language Processing | Skimming Literature | [SkimLit](https://github.com/Infotrend-Inc/CTPO-Demo_Projects/tree/main/SkimLit) |

## Testing a Notebook

On a system with an NVIDIA GPU and docker configured to use it, clone the repo, go into a directory with the notebook you want to try and get a ready-to-use Jupyter Notebook with CUDA, TensorFlow, PyToch and OpenCV available by:

```
docker run --rm -it --runtime nvidia --gpus all -v `pwd`:/iti -p 8888:8888 infotrend/ctpo-jupyter-cuda_tensorflow_pytorch_opencv-unraid:12.3.2_2.16.1_2.2.2_4.9.0-20240421
```

before going to http://127.0.0.1:8888/ and login using the default "iti" password.

