### A deep convolution neural network based Alzheimers analysis and early detection using Magnetic Resonance Imaging.

>* #### **Abstract**
Alzheimer's disease, a cause of dementia that results in gradual brain disorder (loss of memory). It is a neurodegenerative disorder that reasons interactive problems, memory, and feeling, and that ultimately is fatal.  Brain Imaging via magnetic resonance imaging (MRI), is used for evaluation of patients with suspected AD that gives satisfactory resolution of the brain's soft tissues. Traditional computer vision techniques are used in the AD classification process in the recent times. All the methods aid in making decisions, whether an image is an AD or not. But, evolution of deep learning expanded countless devotion in almost every field of computer vision and image processing with inclusion of techniques like feature extraction, exploratory data analysis (EDA).
The main objective is to enhance classification accuracy to get the high-performance prediction of disease that helps us for early detection likely at pre-symptomatic stages that  reduces the occurrence of dementia and prevents the evolution of the disease.


>* #### **Dataset and its description**
The MRI related data that was generated by the Open Access Series of Imaging Studies (OASIS) project that is available both, on their website and kaggle that can be utilized for the purpose of training various machine learning models to identify patients with mild to moderate dementia. The dataset consists of 5 stages of Alzheimer's Disease already split into two directories for training and testing. It focuses on understanding the diagnostic and predictive value of Alzheimer’s disease specific biomarkers. It includes data of 1,500 patients and a total of 1,80,000 images after augmentation.

**Test and Train sets:**
* Mild Cognitive Impairment (MCI)
* Alzheimer's Disease (AD)
* Significant Memory Concern (SMC)
* Early Mild Cognitive Impairment (EMCI)
* Late Mild Cognitive Impairment (LMCI)

We used this dataset to perform binary classification between Non Demented and Mild Demented images. This resource consisted of around 2000 images each, but study used only 200 images from each category. Sequentially, images were preprocessed to resize into (229,229) and 80% images are used as training_data and 20% images as test_data.
We will be using the longitudinal MRI data. The dataset consists of a longitudinal MRI data of 150 subjects aged 60 to 96. Each subject was scanned at least once. 72 of the subjects were grouped as 'Nondemented' throughout the study. 64 of the subjects were grouped as 'Demented' at the time of their initial visits and remained so throughout the study. 14 subjects were grouped as 'Nondemented' at the time of their initial visit and were subsequently characterized as 'Demented' at a later visit. 


>* **#### Methodology**

This model is implemented with the idea of an Intelligent Healthcare Prediction and Classification System for AD Based on Deep learning. The main objective is to enhance classification accuracy to get the high-performance prediction of disease that helps for an early detection of disease reducing the occurrence of dementia. The existing kinds of research still do not show high performance of classification. So, the ultimate goal to improve the accuracy of the model by using Deep Learning.

Deep Learning is the most recent technique that allows the machine to distinct representation from raw data. In traditional machine learning technique is required to identify most of the feature by the expert to minimize data complexity and make it more visible for working with a learning algorithm. Unlike Deep Learning algorithms aims to learn high-level features extraction from data. This removes the need for domain expertise.

To detect Alzheimer's Disease from the MRI scans, (in .nii extension) given as input. It involves several pre-processing steps such as skull stripping, bias correction and segmentation. Once the segmentation is completed, three 2D slices (axial, coronnal, saggital) are extracted from the segmented MRI Image. In this manner the dataset is prepared which is then used for training a simple CNN.
Here, the problem is approached in two methods. One method is to prepare a single dataset wherein the axial,coronnal and saggital images are present within each class which is then fed into a single classifier. Another method is to prepare three datasets (each contain only one kind of data) which is then fed into three classifiers (Axial, Coronnal and Saggital). When compared, it was observed that the combined classifier(Axial,Coronnal,Saggital- 95%) has more accuracy than the single classifier (86%).
