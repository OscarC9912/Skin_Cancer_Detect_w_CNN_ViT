# Skin Cancer Detection with Convolutional Neural Network and Vision Transformer


Skin cancer is a common and deadly disease, and early detection is crucial for successful treatment. In this study, we compare the performance of two deep learning models, the Convolutional Neural Network (CNN) and Transformer, on the task of skin lesion detection. Using diagnostic results from dermatologists in the HAM10000 dataset, we trained the Inception V3 model and Vision Transformer and tested them on the ISIC 2018 challenge test dataset. We found that class imbalance in the training data had a significant impact on model effectiveness, but by employing various methods such as oversampling and focal loss, we were able to address this issue. Our results show that the CNN achieved a two-way accuracy of 81.68\% and an AUC score of 0.89, while the Transformer had an accuracy of 75\% and an AUC score of 0.78. These findings suggest that the CNN is more robust than the Transformer when working with limited data for skin lesion detection.



# File Description

`data_processor.ipynb`: contains code for initial data pre-pocessor for the Dataset

`Skin_Cancer_CNN_ADAM.ipynb`: contains the code for class imbalanced CNN in the paper

`Skin_Cancer_CNN_Paper.ipynb`: contains the code that reproduce the [Esteva et, al.'s paper](https://www.nature.com/articles/nature21056)

`vit_model.ipynb`: contains the code for ViT Model in the paper





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
