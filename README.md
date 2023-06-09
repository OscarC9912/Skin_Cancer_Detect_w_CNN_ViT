# Skin Cancer Detection with Convolutional Neural Network and Vision Transformer


Skin cancer is a common and deadly disease, and early detection is crucial for successful treatment. In this study, we compare the performance of two deep learning models, the Convolutional Neural Network (CNN) and Transformer, on the task of skin lesion detection. Using diagnostic results from dermatologists in the [HAM10000 Dataset](https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000?resource=download), we trained the Inception V3 model and Vision Transformer and tested them on the [ISIC 2018 Challenge Test Dataset](https://challenge.isic-archive.com/data/). We found that class imbalance in the training data had a significant impact on model effectiveness, but by employing various methods such as oversampling and focal loss, we were able to address this issue. Our results show that the CNN achieved a two-way accuracy of 81.68\% and an AUC score of $0.89$, while the Transformer had an accuracy of 75\% and an AUC score of $0.78$. These findings suggest that the CNN is more robust than the Transformer when working with limited data for skin lesion detection.


<img src="https://user-images.githubusercontent.com/74989268/233214451-90e4902e-c447-4029-9986-c616d8dca001.jpg" width="150" height="150"> <img src="https://user-images.githubusercontent.com/74989268/233214996-76a6f781-879b-4ff2-927a-9096cb197c92.jpg" width="150" height="150"> <img src="https://user-images.githubusercontent.com/74989268/233215159-16371f38-36d8-4f12-9f71-8c9a67e5b22b.jpg" width="150" height="150">

# File Description

`data_processor.ipynb`: contains code for initial data pre-pocessor for the Dataset

`Skin_Cancer_CNN_ADAM.ipynb`: contains the code (tensorflow) for class imbalanced CNN in the paper

`Skin_Cancer_CNN_Paper.ipynb`: contains the code (tensorflow) that reproduce the [Esteva et, al.'s paper](https://www.nature.com/articles/nature21056)

`vit_model.ipynb`: contains the code (PyTorch) for ViT Model in the paper




# Contribution:
William Gagné: 
- implement the Convolutional Neural Network
- Responsible for the CNN-related part, conclusion, and the overall polish of the Paper.

Boyuan Cui (Bryan): 
- implement the Vision Transformer (ViT)
- Responsible for the Abstract, ViT-related part, and the reference organization of the Paper.

Zhonghan Chen (Oscar): 
- implement the code for data pre-processing and the dataloader for ViT
- Responsible for the Introduction, Dataset, Model Comparison Analysis, and Appendix organization of the Paper


# Architecture:

![Inception V3](https://user-images.githubusercontent.com/74989268/233217970-cebedc80-bb11-4443-b5e8-412d4ca49f66.png)

![Vision Transformer](https://user-images.githubusercontent.com/74989268/233216076-f82d1f8c-1038-4ccb-a5bc-f32efb3da8ef.png)
