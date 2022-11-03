# Breast Cancer Classification

Current computer-aided diagnosis (CAD) systems are a helpful tool for a radiologist to detect breast cancer. However, decision support system (DSS) evaluation has been challenging due to results that are difficult to reproduce. This originates from the fact that many private datasets have been used in different research, making them hard to compare. The CBIS-DDSM dataset provided by Cancer Imaging Archive is a standardized and updated version of the Digital Database for Screening Mammography (DDSM) that intends to resolve this reproducibility issue. Our research has used this dataset to develop a classifier that classifies mammography images as either benign or malignant. The ResNet architecture has been used because other researchers have had good results with it. Unfortunately, despite our initial ambition, our model fails to classify the images accurately. However, this project lays the foundation for developing a mammography classifier in a reproducible manner.

## Reproduce the results
To reproduce the results one need to do the following steps:

1. Install requirements with `pip install -r requirements.txt`
2. Download full dataset from https://www.kaggle.com/datasets/awsaf49/cbis-ddsm-breast-cancer-image-dataset end extract the images into `archive/jpeg`.
   - Note that the csv files are already included in the repository.
   - The original dataset is also available on the Cancer Imaging Archive with extensive description: https://wiki.cancerimagingarchive.net/display/Public/CBIS-DDSM
3. To structure the images to support flow from directory, run the `preprocess.ipynb` notebook.
4. To train the model, run the `model_training.ipynb` notebook.
5. To evaluate the model, run the `model_evaluation.ipynb` notebook.
