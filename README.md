This repo contains the project code for the CS5242 (Neural Networks & Deep Learning) course taken @ NUS.

Objective:

The primary objective of this project is to develop a classification system capable of distinguishing between five classes of white blood cells: basophil, eosinophil, lymphocyte, monocyte, and neutrophil.

Deep Learning Task:

This Deep-learning task involves the classification of the WBC dataset into five classes. Pre-training is performed  using the PRCC and Camelyon16 datasets, with a portion of the training set accompanied by masks. 
The main objective is to develop an algorithm that uses the additional information from the pre-training datasets to enhance the model's performance on WBC image classification. 
ML task involves experimenting with varying portions of the WBC training set (100%, 50%, 10%, and 1%) to evaluate how the addition of supplementary data from pre-training datasets affects both the training process and overall model performance.

My Implementation:

In this project, I implemented a multi-step process that involved training the PRCC and CAM16 models on their respective datasets separately. 
Subsequently, I trained the white blood cell (WBC) dataset on various proportions of the data (1%, 10%, 50%, 100%). 
Next, I combined the features obtained from the PRCC and CAM16 models and used them to retrain the WBC dataset again on the same proportions of data (1%, 10%, 50%, 100%). 
This approach enabled the integration of knowledge from the pre-trained PRCC and CAM16 models to enhance the classification performance of the WBC dataset, thus increasing class-wise and overall accuracies.

I am training the PRCC and CAM16 models separately and then 
merging their output latent features from them to be integrated 
into the training of the WBC models with varied datasets.
