# MarriagePrediction

## Table of Contents
* Overview/Problem Statement
* Dataset
* File Structure
* Major Packages/Libraries Used
* Installation/Working Environment
* Building the Web App
* Model Deployment on Heroku Platform
* App Implementation
* Drawbacks and Future Scope
* Credits

### 1. Overview/Problem Statement
* Ever wanted to know at what age you will get married? This ML model tries to predict the marriage age using regression techniques.
* For this problem, Linear Regression, Lasso/Ridge Regression, RandomForest and XgBoost algorithms were implemented, RandomForest giving the best results.

### 2. Dataset
* The data was collected from the Datamites team and is available on their Youtube channel. I will link to their github repository below so you can have a look at the dataset.
* The dataset contains the following features: **Id**, **Height**, **Gender**, **Religion**, **Caste**, **Mother-Tongue**, **Current Location**, **Profession**, **Country** and **Age of Marriage**.
* [Dateset Link](https://github.com/ashokveda/ML_deployment_Flask_AWS_marriage_age_prediction/blob/master/age_of_marriage_data.csv)

### 3. File Structure
```
├── Notebook.ipynb 
├── Procfile
├── README.md
├── age_of_marriage_data.csv
├── app.py
├── config.toml
├── credentials.toml
├── marriage.pkl
├── requirements.txt
├── setup.sh
```

### 4. Major Packages/Libraries Used
* pandas 
* numpy
* sci-kit learn
* matplotlib
* seaborn
* streamlit

### 5. Installation/Working Environment
Follow the instructions if you want to run the app from your local computer.
* The app is written using **Python 3.8.5**. You can download it from [here](https://www.python.org/downloads/).You can also download **Anaconda** which is a distribution of python from [here](https://www.anaconda.com/products/individual). I would recommend downloading anaconda since it is very useful as it comes with a lot of python libraries, Jupyter and Spyder IDE.
* Once you are done with the installation, you can clone this repository to your computer and install the required packages and libraries using the following line of code through the command prompt where your local environment is setup.
```
pip install -r requirements.txt
```
### 6. Building the Web App
* The web-app was developed using Streamlit framework which is written in python, suitable for small scale projects such as this one. For more information you can check the offical streamlit website by clicking [here](https://streamlit.io/)
* Basic understanding of streamlit and html was needed for designing the web-app and to make sure it was responsive to user inputs. 

### 7. Model Deployment on Heroku Platoform
* You will have to create a account in order to deploy the model. Login to your account and go to the deploy section.
* Connect to your github repository and deploy the model manually or through Heroku CLI.

![3](https://user-images.githubusercontent.com/83957848/119222443-06092480-bb12-11eb-8102-086761ded15b.JPG)

### 8. App Implementation  
* Link: [MarriagePrediction](https://marriagepredictor99.herokuapp.com/)  
* The app asks for user to enter their Height(Cm), Religion, Caste and Mother-Tongue. Based on these inputs, the age of marriage is predicted.  

![1](https://user-images.githubusercontent.com/83957848/121886360-eccf4e80-cd32-11eb-84b7-f4165144293a.JPG)

### 9. Drawbacks and Future Scope
* A large amount of data was missing and had to be dropped because I could not find any other way of treating the missing values. 
* Some classifier algorithm such as nearest neighbors can be applied to determine the missing data for categorical features.
* Most of the records collected are from Indian background which may lead to biased results.
* The app's front end has room for improvement using CSS or other styling techniques.
* Model performance can be improved.

### 10. Credits
I would like to thank [Ashok Veda](https://github.com/ashokveda) Sir and Datamites team for providing the dataset on their youtube channel, whose work was taken as inspiration for successful completion of this project.  
