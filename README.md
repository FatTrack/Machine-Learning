# C242-PS030 Machine-Learning Path
Proudly presented by Capstone Team

# Table of Contents
1. [Introduction](#introduction)
2. [Components](#components)
3. [Requirements](#Requirements)
5. [Dataset](#dataset)
6. [Workflow](#workflow)
7. [Contributors](#contributor)



## Introduction Project
Fat Track is an AI-based application that helps users monitor their daily food content by recognizing images of food captured by the user and displaying the nutritional content of the food. Fat Track will display information such as calories, protein, fat, and carbohydrates of the food, which will then be stored to track the nutritional intake of the user's daily meals.

Theme : Healthcare


## Components
- Image Pre-processing
- Image Augmentation
- Early Stopping
- Callbacks
- Model Checkpoint
- Convolutional Neural Network (CNN)
- Transfer Learning
  - DenseNet121
  - InceptionV3
  - ResNet152V2
- Model Evaluation
- Accuracy and Loss Graph



## Requirements
| Library             | Version    |
|---------------------|------------|
| tensorflow          | 2.16.1     |
| keras               | 3.3.3      |
| matplotlib          | 3.7.5      |
| numpy               | 1.26.4     |
| pandas              | 2.2.3      |
| scikit-learn        | 1.2.2      |


## Dataset
File Dataset = https://drive.google.com/file/d/1B311xmZPac-LeUwJwfn-qODAzAbdSLAS/view?usp=drive_link

<div align="center">
  <img src="https://github.com/FatTrack/Machine-Learning/blob/main/preview.png" alt="Preview Dataset FatTrack" style="width: 20%;">
  <p></p>
</div>


## Workflow
### 1. Download Images Using Bing Image Downloader
   - Use **Bing Image Downloader** to download images of food based on categories (e.g., satay, rendang, nasi goreng).
   - The images will be saved in a structured folder according to the food category.

### 2. Open the .ipynb File in Google Colab or Jupyter Notebook
   - Open the `.ipynb` file in **Google Colab** or **Jupyter Notebook**.
   - Select **File > Save a copy in Drive** to save a copy of the file to your Google Drive account. This allows you to edit and run the notebook in Google Colab.

### 3. Preprocessing Data
   - Preprocess the downloaded images:
     - **Cleaning**: Remove irrelevant or blurry images.
     - **Resizing**: Resize the images to a standard size (e.g., 224x224 pixels).
     - **Normalization**: Scale the image pixels to the range [0, 1].
     - **Augmentation**: Apply image augmentation techniques such as rotation, flipping, zooming, etc.

### 4. Model Building: Baseline Model (CNN)
   - Build a basic CNN model first as a baseline before moving on to more complex models.

### 5. Transfer Learning Models
   - Implement transfer learning using pre-trained models:
     - **DenseNet121**
     - **InceptionV3**
     - **ResNet152V2**
   - Add custom layers if necessary to adapt the model to your dataset.

### 6. Training the Model
   - Train the model using the preprocessed data.
   - Use **Early Stopping** to halt training if no improvement is seen.
   - Save the best model using **Model Checkpoint**.

### 7. Run Every Cell in the .ipynb File
   - Run each cell in the `.ipynb` file to train the model and produce the desired outputs.
   - Ensure that the process runs without errors and the model is trained correctly.

### 8. Model Evaluation
   - Evaluate the model using relevant metrics such as:
     - Accuracy, Precision, Recall, and F1-Score.
     - Visualize accuracy and loss graphs during training.

### 9. Download the Model .h5 File
   - After training, **download the .h5 model file** by clicking on the `.h5` file in the Colab directory.
   - The model file is automatically saved to the `/content/` directory in Google Colab via **Model Checkpoint**.



## Contributor
| Name                       | Bangkit ID        | University                                |
|----------------------------|-------------------|-------------------------------------------|
| Ahmad Ferdiansyah           | M211B4KY0204      | Universitas Indraprasta PGRI              |
| Arif Adrian                 | M319B4KY0637      | Universitas Sumatera Utara                |
| Ikko Cahya Awinata          | M284B4KX1925      | Universitas Negeri Surabaya               |


