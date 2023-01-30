# multi-class-brain-tumor-classification

This repository contains the code of the paper
### Multi-class classification of brain tumor types from MR Images using EfficientNets
Fatima Zulfiqar, Usama Ijaz Bajwa, Yasar Mehmood

## Abstract
Accurate classification of the type of brain tumor plays an important role in the early diagnosis of the tumor which can be the difference between life and death. Magnetic Resonance Imaging (MRI) is commonly used to capture high-contrast grayscale images of the brain and is a non-invasive method for brain tumor diagnosis. Deep Learning (DL) using Convolutional Neural Networks (CNN) has revolutionized Computer Aided Diagnostic (CAD) systems by producing remarkable results for various medical imaging analysis tasks including brain tumor detection. In this research, a transfer learning-based fine-tuning approach for the classification of brain tumors into three classes i.e. glioma, meningioma, and pituitary tumor using EfficientNets is carried out. Five variants of pre-trained models from the EfficientNets family i.e.  EfficientNetB0 – EfficientNetB4 are fine-tuned on publically available CE-MRI “Figshare – Brain Tumor Dataset”. The proposed method of fine-tuning pre-trained EfficientNet is carried out by first loading ImageNet weights to the EfficientNet model followed by the addition of several top layers and a fully connected layer for the classification of brain tumor types. Several experiments are carried out to analyze the robustness of the proposed fine-tuned EfficientNets in comparison to other pre-trained models. Moreover, the effect of data augmentation on the model’s test accuracy is also studied. Finally, the Grad-CAM visualization of the attention maps of the best model is presented that successfully highlights the tumorous region of the brain cell. The proposed method of fine-tuning pre-trained EfficientNet showed significant performance using EfficientNetB2 as a backbone achieving overall test accuracy, precision, recall/sensitivity, and F1-score of 98.86%, 98.65%, 98.77%, and 98.71% respectively. The proposed fine-tuned EfficientNetB2 is lightweight, computationally inexpensive (during training and inference), and generalizes well.

## Dataset
Dataset can be downloaded from the following link <br>
(https://figshare.com/articles/dataset/brain_tumor_dataset/1512427)

# Steps
1. Crop brain contour
2. Use https://github.com/jfilter/split-folders to split dataset into train and test of 80:20
3. Apply Data augmentation on dataset in train set only
4. Train model and evalaute
