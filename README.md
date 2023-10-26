# My Data Science / Machine Learning Portfolio

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

## Current Projects

### [Project: House Price Predictor using Linear Regression](https://github.com/SHAKyMLRepo/Project1-HousePricePrediction.git)* 

#### Introduction

The real estate market is a dynamic and complex environment, and predicting house prices accurately is a valuable tool for homeowners, buyers, and real estate professionals. This project aims to explore the links between property prices, population and population density. It aims to try and establish the degree of correlation between such factors and determine if it is possible to estimate how house prices will behave into the future based on factors such as land area, population and population density.

#### Project Overview

**Objective**: The primary objective of this project is to create a House Price Prediction algorithms that employs Linear Regression to estimate the selling price of houses based on the available land space in a region and its population density.

**Key Components**:

1. **Data Sourcing**: In this project, I sourced publically available datasets with the necessary information required to begin to develop the inputs for this project. This proved to be a challenging task as while there is plenty of high quality data on Irish Population statistics, due to privacy concerns many of the publically avaiable datasets regarding House Prices cannont contain any PII so have many of the fields you might wish for to answer these questions removed or lowered in fidelity to protect privacy. In the end, a number of seperate datasets were required to collate the fields necessary for the project.

2. **Data Preprocessing**: As this project could not use a prepared dataset as none was available with the information required regarding the Irish market, the Data Preprocessing stage was one of the most involved stage of this project. This involved tasks such as handling missing values, dealing with outliers, and removing unneeded data. As multiple datasets had to be combined it also required datasets formats to be synchronised before combination. The goal was to prepare the data for model development by ensuring it was clean and structured.
   
3. **Model Development**: Implement a Linear Regression model using the machine learning library Scikit-Learn. Train the model on the prepared dataset to learn the relationships between the selected factors and house prices.

4. **Model Evaluation**: Evaluate the performance of the Linear Regression model a subset of the data which will be held back during training.

5. **User Interface**: Create a simple text interface to allow Users to query the model.


**Benefits**:

- **Accurate Predictions**: The project offers a reliable tool for estimating house prices based on various factors and explores the weight by which different factors effect house prices into the future. 

- **Data-Driven Insights**: Users can gain insights into the factors influencing house prices, helping them make informed choices.

- **Real-World Application**: The project demonstrates the application of machine learning in a real-world scenario and highlights the potential for predictive modeling in the real estate industry based on population dynamics.

**Ethics and Regulations**:

- **Data Privacy and GDPR Compliance**: The data from this project should have no PPI included so will not have GDPR compliance implications.

- **Data Attribution and Terms of Use**: The project will use publically available datasets and will give full attribution of the data sets used  and comply with any terms of use.

### [Project: Automated Data Scraping from Weather Website and storage to a local database](https://github.com/SHAKyMLRepo/Project2.git)*

#### Introduction

In a world increasingly reliant on data-driven decision-making, access to accurate and up-to-date weather information is crucial for various applications, from agriculture to logistics and personal planning. This project aims to hone my skills in data scraping data from a website. This data will be in an unstructured state so data cleaning and transformation skills will also be required. This process of will retrieve, clean and transform the data automatically and then store it in a local database for easy access and analysis.

#### Project Overview

**Objective**: The primary goal of this project is to automate the retrieval of weather data from a selected weather website and establish a local database to store this data efficiently.

**Key Components**:

1. **Web Scraping**: We will develop a web scraping script using the BeautiSoup library to extract the weather data (e.g., temperature, humidity, wind speed, and conditions) from the weather website. This script will run at specified intervals to keep the data up to date.

2. **Data Transformation**: Once the data is scraped, it will be transformed and structured into a format suitable for database storage. This step may involve data cleaning and formatting.

3. **Local Database**: We will set up a local database using SQLite to store the scraped weather data. The database schema will be designed to accommodate the specific data attributes.

4. **Automation**: The entire process will be automated, with scheduled runs of the web scraping script to keep the database updated with the latest weather information.

5. **Data Access**: Users will be able to access and query the local database for weather information.

**Benefits**:

- **Data Availability**: Weather data will be readily available in a local database, reducing the need for real-time API calls to external sources.

- **Data Analysis**: With data stored locally, I intend to use this data in future projects.

**Ethics and Regulations**:

- **Data Privacy and GDPR Compliance**: The data from this project should have no PPI included so will not have GDPR compliance implications.

- **Website Terms of Use**: As we are web scraping from commercial websites, we must ensure we comply with their terms of use. This project is just for personal development of Data Scraping and Data Cleaning skills and will not be used for commercial activity due to these terms. The project will transparently state the source and owner of the data with clear attribution.

### [Project: Webpage with Weather Chatbot using Local Database](https://github.com/SHAKyMLRepo/Project3.git)* 

#### Introduction

In an era where technology is becoming increasingly integrated into our daily lives, having a chatbot that can provide weather forecasts in a conversational manner can be a valuable asset. This project aims to develop my skills with the creation of chatbots and builds off the project above. The chatbot will retrieve weather data from a local database and respond in a human-like text format.

#### Project Overview

**Objective**: The main objective of this project is to develop a web-based chatbot that can provide weather forecasts based on user queries and data stored in a local database.

**Key Components**:

1. **User Interface**: A web page will be created to serve as the user interface. Users can input their queries about the weather through a prompt or chatbox.

2. **Chatbot Development**: The chatbot will be designed to understand natural language queries related to weather forecasts. It will utilize Natural Language Processing (NLP) techniques to process and interpret user inputs.

3. **Local Database Integration**: Weather data, previously collected from a weather website and stored in a local database as part of a previous project, will be used by the chatbot to provide responses. The chatbot will query the database to retrieve weather forecasts for specific dates.

4. **Conversational Responses**: The chatbot will respond to user queries in a conversational and human-like manner. Responses will include weather conditions, temperatures, and any other relevant information for the specified date.

5. **Web Interaction**: Users will interact with the chatbot through the web page, where they can ask questions like, "What will the weather be like on [specific date]?" The chatbot will generate informative and user-friendly responses.

**Benefits**:

- **User-Friendly Access**: The web-based chatbot provides an easy and intuitive way for users to inquire about weather forecasts without needing to navigate complex interfaces or APIs.

- **Conversational Experience**: Users can have a natural conversation with the chatbot, making the interaction more engaging and user-friendly.

- **Data Utilization**: The project leverages previously collected weather data, making efficient use of data already available in the local database.

- **Integration Potential**: The chatbot can be further expanded and integrated into other platforms or applications to provide weather information seamlessly.

**Ethics and Regulations**:

- **Data Privacy and GDPR Compliance**: The data from this project should have no PPI included so will not have GDPR compliance implications.

- **Data Attribution and Terms of Use**: The project will transparently state the original source and owner of the data with clear attribution and will not be used in any commercial context.

*Feel free to reach out through LinkedIn if you'd like more details or have any questions about my projects or skills!*
