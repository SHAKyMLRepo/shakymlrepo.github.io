# Data Science / Machine Learning Portfolio

![ML Banner](Images/mlbanner.jpg)

## About Me

I am a fourth-year student at SETU, Carlow, with a strong passion for Machine Learning. My interests in Machine Learning include Object Identification, Image Processing, and Chatbots. I am at the beginning of my Machine Learning journey but enthusiastic about learning and completing projects to further my skills and knowledge.

## Experience
Worked for six months as an Intern in the Enterprise Data department of Unum Ireland. Here I got to develop skills in a broad range of Data Science skills including Data Cleaning, Data Analysis and Data Pipelines. Some of the Projects I worked on during that time were the creation of a Data Pipeline to automate the building of reference tables for one of their Data Warehouses and an Intern led project which created a Data Analysis Dashboard of live data from one of Unum's Enterprise application.

## Skills

#### Infrastructures
- Cloud Computing (AWS, PythonAnywhere)
- Docker and Containerization
- Virtualization (VMware, VirtualBox)

#### Data and Data Storage Technologies
- SQL and Relational Databases (Teradata, MariaDB, Microsoft SQL Server)
- NoSQL Databases (MongoDB)
- Data Warehousing (Teradata)
- Data Pipelines (MongoDB Aggregations, IBM Datastage, Tableau Prep)

#### Data Analysis
- Data Visualisation (Tableau)

#### Programming Languages
- Python (BeautiSoup, Pandas)
- Java
- JavaScript
- React, React native
- C++, C
- X86 Assembly

#### Machine Learning Algorithms
- Linear Regression

#### Other Technical Skills
- Git and Version Control
- Linux/Unix Systems
- Web Development (HTML, CSS, Flask, Anvil, React)
## Semester 2 Projects

### [Project 1: Spam Detection using Naive Bayes Classifier](https://github.com/SHAKyMLRepo/Project-4-Spam-Detection-using-Naive-Bayes-Classifier)

### [Project 2: Detection of Glasses in Images using Support Vector Machines](https://github.com/SHAKyMLRepo/Project-5-Glasses-Detection-using-Support-Vector-Machines)

### [Project 3: Heart Disease Prediction using K Nearest Neighbours](https://github.com/SHAKyMLRepo/Project-6-Heart-Disease-Prediction-using-K-Nearest-Neighbours)

### [Project 4: Spotify Recommendations using K Means Clustering](https://github.com/SHAKyMLRepo/Project-7-Spotify-Recommendations-using-KMeans-Clustering)

### [Project 6: Animal Image Classification using CNNs](https://github.com/SHAKyMLRepo/Project-8-Animal-Image-Classification-using-CNNs)

## Current Projects

### [Project: House Price Predictor using Linear Regression](https://github.com/SHAKyMLRepo/Project1-HousePricePrediction.git)* 

#### Introduction

The real estate market is a dynamic and complex environment, and predicting house prices accurately is a valuable tool for homeowners, buyers, and real estate professionals. This project aims to explore the links between property prices, population and population density. It attempts to establish the degree of correlation between such factors and determine if it is possible to estimate how house prices will behave into the future based on factors such as land area, population and population density.

#### Project Overview

**Objective**: The primary objective of this project is to create a House Price Prediction algorithm that employs Linear Regression to estimate the selling price of houses based on the available land space in a region and its population density.

**Key Components**:

1. **Data Sourcing**: In this project, I sourced publically available datasets with the necessary information required to begin to develop the inputs for this project. This proved to be a challenging task as while there is plenty of high quality data on Irish Population statistics, due to privacy concerns many of the publically avaiable datasets regarding House Prices cannont contain any PII so many of the fields you might wish to obtain to answer these questions are often removed or lowered in fidelity to protect privacy. In the end, a number of seperate datasets were required to collate the fields necessary for the project.

2. **Data Preprocessing**: As this project could not use a prepared dataset as none was available with the information required regarding the Irish market, the Data Preprocessing stage was one of the most involved stages of this project. As multiple datasets had to be combined it required many datasets to be combined. Each dataset first required the handling missing values, dealing with outliers, and removing unneeded data. Formats then needed to be synchronised to enabled accurate joining. The goal was to prepare the data for model development by ensuring it was clean, structured and contained the necessary fields.
   
3. **Model Development**: The machine learning library SKLearn was utilised in this project to implement the Linear Regression model. Due to the dataset contained categorical fields, a column transformer was used with OneHotEncoding to concert these fields to numerical values. The data was then split into training and test sets to enable model evaluation. The model was then trained on the prepared dataset to learn the relationships between the selected factors and house prices.

4. **Model Evaluation**: Evaluate the performance of the Linear Regression model a subset of the data which will be held back during training.

5. **User Interface**: Create a simple text interface to allow Users to query the model.


**Benefits**:

- **Accurate Predictions**: The project offers a reliable tool for estimating house prices based on various factors and explores the weight by which different factors effect house prices into the future. 

- **Data-Driven Insights**: Users can gain insights into the factors influencing house prices, helping them make informed choices.

- **Real-World Application**: The project demonstrates the application of machine learning in a real-world scenario and highlights the potential for predictive modeling in the real estate industry based on population dynamics.

**Ethics and Regulations**:

- **Data Privacy and GDPR Compliance**: The data from this project should have no PPI included so will not have GDPR compliance implications.

- **Data Attribution and Terms of Use**: The project will use publically available datasets and will give full attribution of the data sets used  and comply with any terms of use.

If you wish to learn more about this project, click the title link to view its repository on GitHub. More detailed information can be found in the projects Readme.md file and you can view the project code to gain further insights.

### [Project: Face Mask Detection using Convolutional Neural Network (CNN)](https://github.com/SHAKyMLRepo/Project2-Face-Mask-Detection-using-CNN.git)

#### Introduction

The rapid advancement of Computer Vision technology has opened many new uses cases in recent years and this project aims to leverage these new technology and explore their application in the solving of  real world problems. The goal is to develop a Convolutional Neural Network (CNN) capable of accurately identifying whether an individual in an image is wearing a face mask or not. This technology has direct applications in public spaces, healthcare facilities, and various sectors where adherence to mask-wearing guidelines is crucial.

#### Project Overview

**Objective**: The primary objective of this project is to build a robust Face Mask Detection model using Convolutional Neural Network techniques. The model aims to analyze images and determine whether the person in the image is wearing a face mask.

**Key Components**:

1. **Data Collection**: This project utilizes a prepared dataset sourced from Kaggle, consisting of images containing individuals with and without face masks. The dataset was chosen for its comprehensiveness, diversity, and the availability of labeled data. While traditional data collection involved capturing real-world scenarios, lighting conditions, and backgrounds, using a curated Kaggle dataset streamlines the process and ensures access to a high-quality, labeled dataset.

2. **Data Preprocessing**: The dataset underwent exploratory data analysis and visualization to ensure suitability. A dedicated function was developed to iterate through images and reshape them to conform to the models imput layer requirements. The function then created a list of arrays contained an image and label into the form of a binary value  (0 for without mask, 1 for with mask). The dataset was then split into training, validation, and test sets for effective model evaluation.

3. **Model Development**: The Keras library from Tensorflow was used for model developement by leveraging a pretrained model from that library and then using transfer learning to hone its parameters to the requirements of this task. This method saves on both training time and processing power required for model training. The model architecture was chosen to be as lightweight as possible to be capable of deployment to lower power devices with the aim of validating possible integrations to low resource devices such as CCTVs cameras. Training was conducted usings the prepared dataset over multiple epochs to achieve high accuracy in face mask detection.

4. **Model Evaluation**: The trained model will be evaluated on a separate test dataset to assess its performance in terms of precision, recall, and overall accuracy.

5. **User Interface or Deployment**: Depending on the project scope, a user-friendly interface may be developed to allow users to upload images for real-time face mask detection. Alternatively, the model can be deployed in applications for automated monitoring.

**Benefits**:

- **Public Health Safety**: The project directly contributes to public health safety by providing a tool to identify individuals not adhering to mask-wearing guidelines.

- **Automation in Monitoring**: The technology allows for automated monitoring in public spaces, reducing the need for manual intervention.

- **Versatile Applications**: Beyond pandemic scenarios, the model can find applications in various settings where mask detection is relevant, such as security and healthcare.

**Ethics and Regulations**:

- **Privacy Considerations**: The project emphasizes privacy by not collecting or storing personally identifiable information. The focus is solely on the presence or absence of face masks.

- **Algorithmic Fairness**: Efforts will be made to ensure that the model's predictions are fair and unbiased across different demographics.

If you wish to learn more about this project, click the title link to view its repository on GitHub. More detailed information can be found in the projects Readme.md file and you can view the project code to gain further insights.


### [Project: Drug Prescription Prediction using Decision Trees](https://github.com/SHAKyMLRepo/Project3-DrugEffectivenessClassifier.git)

#### Introduction

The Drug Prescription Prediction project utilizes Decision Trees to analyze a dataset of drug prescriptions. The primary goal is to leverage machine learning to predict the most suitable drug for a patient based on various health and personal characteristics such as gender, age, blood pressure, and other relevant factors. This project has significant implications for personalized medicine and optimizing drug prescription practices.

#### Project Overview

**Objective**: The main objective of this project is to develop a Decision Tree model capable of accurately predicting the most appropriate drug for a patient based on their health and personal characteristics.

**Key Components**:

1. **Data Collection**:  The Data Collection process for this task was straightfoward as due to privacy concerns and regultations regarding the use of real patient information, a Datatset from Kaggle designed to train such models was utilised for this project.This dataset will be used to generate a proof of concept algorithm to show how such a model could be used in the future using real patient data to make accurate prescription predictions.

2. **Data Preprocessing**: As the dataset came already cleaned and structured, the first tasks in the Preprocessing stage was in Data Exploration and Data Visualisation. In this step, the dataset structure was explored to confirm its suitablilty and Data Visualisations were prepared to gain insight into its contents and assess any problems. Once these steps were complete the dataset was checked for any missing values and the dependent and independent variables identified. The data was then transformed into a feature vector and a target value and these were then split two two sets each, a training set and a test set which will be used later for model evaluation.
the
3. **Model Development**: Implement a Decision Tree algorithm to learn the relationships between patient characteristics and drug prescriptions. Fine-tune the model to achieve optimal performance in predicting drug choices.

4. **Model Evaluation**: Assess the Decision Tree model's performance on a separate test dataset. Evaluate metrics such as accuracy, precision, and recall to measure the model's effectiveness in drug prescription prediction.

5. **User Interface or Deployment**: A simply text interface will be devloped which will serve as a proof of concept interface where drug predictions can be viewed based on a Users input parameters. This interface will show how such an algorithm could be used by real healthcare professionals to speed up their drug prescription procedures..

**Benefits**:

- **Personalized Medicine**: The project contributes to the advancement of personalized medicine by providing a tool for tailoring drug prescriptions based on individual patient characteristics.

- **Efficient Healthcare Practices**: Healthcare professionals can benefit from more efficient and informed decision-making in drug prescription, leading to better patient outcomes.

- **Data-Driven Healthcare**: The project showcases the potential of data-driven approaches in healthcare, optimizing the prescription process.

**Ethics and Regulations**:

- **Patient Privacy**: The project prioritizes patient privacy by utilising mock data, protecting patient privacy and ensuring compliance with healthcare regulations.

- **Transparency in Model Decisions**: Efforts will be made to ensure transparency in the Decision Tree model's decisions, providing insights into the factors influencing drug prescription predictions.

If you wish to learn more about this project, click the title link to view its repository on GitHub. More detailed information can be found in the projects Readme.md file and you can view the project code to gain further insights.

*Feel free to reach out through LinkedIn if you'd like more details or have any questions about my projects or skills!*
