#  Flower Classification

## Overview
This project involves the classification of images of flowers using deep learning models. The team experimented with several popular models such as ResNet, DenseNet, and MobileNet to improve the accuracy of image classification tasks. The project is developed as part of COMP6721 in the Fall 2024 semester.
<br />
<br />

## Datasets
Datasets | Auther | Links |
| ------------- | --------- | ------------ |
| Flower Classification \| 5 Classes | utkarshsaxenadn | <a href="https://www.kaggle.com/datasets/utkarshsaxenadn/flower-classification-5-classes-roselilyetc">*kaggle*</a> |
| 🌸 \| Flower Classification | marquis03 | <a href="https://www.kaggle.com/datasets/marquis03/flower-classification">*kaggle*</a> |
| flowers | nadyana | <a href="https://www.kaggle.com/datasets/nadyana/flowers">*kaggle*</a> |

<hr />
<br >

## Folder Structure
The project folder has the following structure:

```
COMP6721_Winter2023_GroupO
├── Docs
│   ├── MobileNetV2/  
│   ├── ResNet18/
│   ├── Project_Proposal_Group_O.pdf
│   └── Project_Report_Group_O.pdf
│
├── notebooks
│   ├── Extra/
│   ├── resnet_5.ipynb
│   ├── resnet_7.ipynb
│   ├── resnet_14.ipynb
│   ├── mobilenet-5.ipynb
│   ├── mobilenet_7.ipynb
│   ├── mobilenet_14.ipynb
├── LICENSE
├── .gitignore
├── README.md
└── requirements.txt
```
### <li>Notebooks
This folder contains `Jupyter notebooks` used for machine learning experiments with various models. These notebooks are compatible with `Google Colab`, `Jupyter Notebooks`, and `Kaggle`. 
>**Note:**
>*To use these notebooks, you `must install all the required libraries` mentioned in the ```requirements.txt``` file in your environment and place the datasets in the appropriate location, or adjust the folder path mentioned in the code accordingly.*
  
### <li>Docs
This folder contains all the project documents created by the team. These include the project proposal and the final project report.


### <li>LICENSE:
This file contains the license under which the software in this repository is released. It is important to read and understand the license before using or distributing any code or other materials in this repository.

### <li>requirements.txt:
This file contains a list of all the Python packages that are required to run the notebooks in this repository. 
>**Note:**
>*You can install the required libraries by running the following command in your terminal or command prompt:*
``` 
pip install -r requirements.txt
```

<hr />

<br />

## How to run the code
>**Note:**
> *If you want to train the model from the scratch follow the bellow steps:*

1. Clone the repository to your local machine using the following command:
```
git clone https://github.com/AbhiMavani/COMP6721-GroupU
```
2. Install the required dependencies using the following command:
```
pip install -r requirements.txt
```
3. Launch Jupyter Notebook using the following command:
```
jupyter notebook
```
4. Navigate to the notebooks directory in your Jupyter Notebook dashboard and open the `.ipynb` file.

5. Run the notebook by clicking on the "Run" button or by using the "Shift + Enter" keyboard shortcut.

>**Note:**
>*The dataset used in the notebook can be found on the `Kaggle`. The links for that are mentioned above.*

>**Note:**
>*Its is convineint for you to run this noptebooks on `kaggle` as you dont have to download the datasets or in the `google Colab`.*

<hr />
<br>

## How to Test the model
>**Note:**
> *If you do not want to train the model from the scratch and just have to test the pretrained model then follow the bellow steps:*

1. Load the `'ModelTesting.ipynb'` file from the `'notebooks'` folder, which contains the testing code for the model.

2. Provide the input path of the trained model in the `'torch.load()'` function, which will load the model for testing purposes.

3. A dictionary named `'sat_map'` has been defined for the `dataset-1`, which can be used to convert the predicted output to class labels. Similar dictionaries can be created for other datasets as well.

4. To pass an image for classification, simply provide the path of the image in the `'image.open()'` method, which will open the image for processing.

5. Execute the code to obtain the prediction for the input image.

<br>
<hr />

## Summary of the generated models

|               | Resnet-18 |              |        | Mobilenet-V2 |              |        | Densenet121    |              |        |
| ------------- | --------- | ------------ | ------ | ------------ | ------------ | ------ | --------- | ------------ | ------ |
|               | D1        | D2           | D3     | D1           | D2           | D3     | D1        | D2           | D3     |
| Accuracy (%)  | 83     | 85       | 82  | 87 | 87 | 92 | - | - | - |
| Precision (%) | 82        | 87           | 85     | 88 | 87 | 94 | - | - | - |
| Recall (%)    | 87        | 85           | 82     | 88 | 87 | 92 | - | - | - |
| F1 score      | 83        | 85           | 81     | 88 | 86 | 92 | - | - | - |