<a id="top"></a>
<div style="display:none;" align="center">
<h1><font size="10"> AgroTech AI </font></h1>

<!-- repo intro -->

</div>
<div align="center">

<h3><font size="4">AgriTech AI platform is a comprehensive web-based tool where users can access various machine learning models for making accurate predictions related to agriculture. It offers solutions for crop management, soil health assessment, pest control, and more.</h3>
<br>
Make sure you star the repository and show your love to us💗
</font>
<br>
<br>
<p>

## 📈 GitHub Repository Stats
| 🌟 **Stars** | 🍴 **Forks** | 🐛 **Issues** | 🔔 **Open PRs** | 🔕 **Closed PRs** | ✅ **Contributors** |
|--------------|--------------|---------------|-----------------|------------------|------------------|
| ![GitHub stars](https://img.shields.io/github/stars/gdgmit/AgriTech-AI) | ![forks](https://img.shields.io/github/forks/gdgmit/AgriTech-AI) | ![issues](https://img.shields.io/github/issues/gdgmit/AgriTech-AI?color=32CD32) | ![pull requests](https://img.shields.io/github/issues-pr/gdgmit/AgriTech-AI?color=FFFF8F) | ![Closed PRs](https://img.shields.io/github/issues-pr-closed/gdgmit/AgriTech-AI?color=20B2AA) | ![Contributors](https://img.shields.io/github/contributors/gdgmit/AgriTech-AI?color=00FA9A) |



## Why to Open Source

Contributing in open source increases your opportunities to work with different projects and mentors, getting to know various insights and ideas. It is a platform where contributors grow together with a construvtive and a positive attitude.
This repository also provides one such platforms where contributers come over and put their ideas  and make our website as interactive as much they can!

![GitHub issues](https://img.shields.io/github/issues/gdgmit/AgriTech-AI)
![GitHub forks](https://img.shields.io/github/forks/gdgmit/AgriTech-AI)
![GitHub pull requests](https://img.shields.io/github/issues-pr/gdgmit/AgriTech-AI)
![GitHub Repo stars](https://img.shields.io/github/stars/gdgmit/AgriTech-AI)
![GitHub contributors](https://img.shields.io/github/contributors/gdgmit/AgriTech-AI)

</p>

</div>

<details>
    <summary><h2>:pushpin:Table of Contents: </h2></summary>

## Table of Contents

1. [Project Description](#project-description)
2. [Getting Started / Installation](#getting-started--installation)
3. [API Documentation](#api-documentation)
   - [Fertilizer Prediction](#fertilizer-prediction)
   - [Crop Prediction](#crop-prediction)
   - [Soil Quality Prediction](#soil-quality-prediction)
   - [Yield Prediction](#yield-prediction)
   - [Mushroom Edibility Prediction](#mushroom-edibility-prediction)
4. [Tech Stack](#tech-stack)
5. [Contributing](#contributing)
6. [Code of Conduct](#code-of-conduct)
7. [License](#license)
8. [Stargazers](#stargazers)
9. [Forkers](#forkers)

</details>

<hr>


## Project Description

AgroTech AI platform is a comprehensive web-based tool where users can access various machine learning models for making accurate predictions related to agriculture. It offers solutions for crop management, soil health assessment, pest control, and more.

It implements machine learning algorithms to implement 3 basic functionalities:
### 1. Fertilizer Prediction
Aims to predict the appropriate fertilizer based on environmental and soil conditions. The dataset contains various features like temperature, humidity, moisture, soil type, crop type, and the levels of nitrogen, potassium, and phosphorus in the soil. The model aims to recommend the correct fertilizer to use, improving crop yield and soil health.
 
### Dataset: 
Fertilizer Prediction.csv (Uploaded under notebooks)
 
### Model Development :
A Random Forest Classifier was chosen as the primary model due to its robustness and high accuracy in classification tasks. The dataset was split into training and testing sets in an 80:20 ratio.
Key steps:

#### Label Encoding: 
Categorical variables (Soil Type, Crop Type, and Fertilizer Name) were encoded using LabelEncoder.
#### Model Training: 
A Random Forest model was trained using the training data.
#### Hyperparameter Tuning: 
A grid search with cross-validation was applied to find the optimal parameters for the Random Forest model.

### 2. Crop Prediction
Develop a machine learning-based crop recommendation system that uses various classification algorithms to predict the optimal crop for farming based on soil and environmental factors. The model takes inputs such as Nitrogen (N), Phosphorus (P), Potassium (K), temperature, humidity, pH level, and rainfall, and outputs the most suitable crop for specific conditions.
#### Dataset:
Crop_recommendation.csv

#### Model Training and Results
Four different models were trained on the dataset to predict the crop:
The results of each model are as follows:

1. Logistic Regression: 96.18%
2. Decision Tree Classifier: 97.82%
3. Gaussian Naive Bayes: 99.45%
4. Random Forest Classifier: 99.45%
The final model selected for deployment is the Random Forest Classifier.

### 3. Soil Quality Prediction 
Implements machine learning models to classify soil quality based on various features like nitrogen content, pH levels, organic carbon, and other nutrients. The goal of the model is to predict the quality of soil using logistic regression and a Support Vector Machine (SVM) model.

#### Dataset:
Soil_Quality.csv (Uploaded under notebooks)

#### Model Traning and Results
1. Logistic Regression
Logistic Regression is used to model the soil quality based on the provided features. The dataset is split into training and testing sets, and the logistic regression model is trained on the training data.

2. Support Vector Machine (SVM)
A Support Vector Machine with an RBF (Radial Basis Function) kernel is trained as an alternative model. The SVM model aims to find the decision boundary that best separates different soil quality classes.

3. Performance Evaluation
The performance of both models is evaluated using accuracy. The accuracy of each model is calculated by comparing the predicted soil quality labels with the actual labels in the test dataset.

### 4. Yield Prediction
Aims to develop a machine learning-based model for predicting crop yields based on various environmental and agricultural factors. The primary objective of this project is to create a model that predicts the total crop yield for a given region using data such as Area and type of crop, Year of cultivation, Average rainfall (in mm per year), Pesticide usage (in tonnes), Average temperature (in °C)

#### Dataset:
yield_df.csv (Uploaded under notebooks)

#### Model Training and Results
Various machine learning regression algorithms are applied, and the performance is evaluated based on metrics like Mean Squared Error (MSE).
The results of the models used are as follows:
1. Linear Regression
Mean Squared Error : 80852.08620158922
Score 0.09879301553673503

2. K Neighbors Regressor
Mean Squared Error : 55183.1146293406
Score 0.5801883304861266

3. Decision Tree Regressor
Mean Squared Error : 13211.190235825037
Score 0.9759383181169221

4. Random Forest Regressor
Mean Squared Error : 10135.46523142438
Score 0.9858378410451943

5. Gradient Boosting Regressor
Mean Squared Error : 34773.822585474634
Score 0.833295640875001

6. XGB Regressor
Mean Squared Error : 13451.947664464684
Score 0.975053338957936Linear Regression
Mean Squared Error : 80852.08620158922
Score 0.09879301553673503

The Random Forest Regressor was found to have the lowest MSE, making it the most suitable model for crop yield prediction. This model was selected for deployment and future predictions.

### 5. Mushroom Edibility Prediction
Develop a machine learning model that predicts whether a mushroom is edible or not, depending on it's physical features and environment. The model takes various inputs regarding the physical characteristics of the mushroom and outputs if the mushroom is edible or poisonous.

#### Dataset:
mushrooms.csv

#### Model Training and Results
Five different models were trained on the dataset to predict mushroom edibility. The accuracy of each model are as follows:

1. Logistic Regression: 0.94
2. Decision Tree Classifier: 1.0
3. K Nearest Neighbors: 0.99
4. Random Forest Classifier: 1.0
5. XGB Classifier: 1.0

The final model selected for deployment is the XGBoost Classifier as it can handle missing datas better than the other models.

## TechStack

- React
- Tailwind
- python - Flask
- Node
- MongoDB
- Express
- Machine Learning
- Deep Learning

<hr>

## ⚙️ Getting Started / 📥 Installation

Ready to contribute to this fun project? Here's how to set up your development environment:
<br>
Make sure you follow our contributing guidlines:-  [here](https://github.com/RamakrushnaBiswal/PlayCafe/blob/main/CONTRIBUTING.md) 

1. **Fork this repository** 🍴 and clone it to your local machine:
   ```bash
   git clone https://github.com/gdgmit/AgriTech-AI.git
## ⚙️ Getting Started with Agro Tech AI main website

2. **Install the node modules in frontend directory:**
   ```bash
   npm install
3. **Start the react server ⚡:**
   ```bash
   npm run dev
4. **Install the node modules for backend directory 🧩:**
   ```bash
   npm install
5. **Run the backend server ⚡:**
   ```bash
   npm start
6. Open your browser at `http://localhost:5173` to see the project running! 🌟

## API Documentation

The API provides endpoints for various functionalities of the AgroTech AI platform. Below is a brief overview of the available endpoints:

### 1. Fertilizer Prediction
- **Endpoint:** `/api/fertilizer`
- **Method:** `POST`
- **Request Body:**
  ```json
  {
      "temperature": <number>,
      "humidity": <number>,
      "moisture": <number>,
      "soil_type": "<string>",
      "crop_type": "<string>",
      "nitrogen": <number>,
      "potassium": <number>,
      "phosphorus": <number>
  }
  ```
#### 2. Crop Prediction

- **Endpoint:** `/api/crop`
- **Method:** `POST`
- **Request Body:**
    ```json
    {
        "nitrogen": <number>,
        "phosphorus": <number>,
        "potassium": <number>,
        "temperature": <number>,
        "humidity": <number>,
        "ph_level": <number>,
        "rainfall": <number>
    }
    ```
#### 3. Soil Quality Prediction

**Endpoint:** `/api/soil-quality`  
**Method:** `POST`  

**Request Body:**
```json
{
    "nitrogen": <number>,
    "ph": <number>,
    "organic_carbon": <number>,
    "other_nutrients": {
        "phosphorus": <number>,
        "potassium": <number>
    }
}
```
#### 4. Yield Prediction

**Endpoint:** `/api/yield`  
**Method:** `POST`  

### Request Body:
```json
{
    "area": <number>,
    "crop_type": "<string>",
    "year": <number>,
    "rainfall": <number>,
    "pesticide_usage": <number>,
    "average_temperature": <number>
}
```
#### 5. Mushroom Edibility Prediction

**Endpoint:** `/api/mushroom`  
**Method:** `POST`  

### Request Body:
```json
{
    "cap_shape": "<string>",
    "cap_surface": "<string>",
    "cap_color": "<string>",
    "bruises": "<string>",
    "odor": "<string>",
    "gill_attachment": "<string>",
    "gill_spacing": "<string>",
    "gill_size": "<string>",
    "gill_color": "<string>",
    "stalk_shape": "<string>",
    "stalk_surface_above_ring": "<string>",
    "stalk_surface_below_ring": "<string>",
    "stalk_color_above_ring": "<string>",
    "stalk_color_below_ring": "<string>",
    "veil_type": "<string>",
    "veil_color": "<string>",
    "ring_number": "<string>",
    "ring_type": "<string>",
    "spore_print_color": "<string>",
    "population": "<string>",
    "habitat": "<string>"
}
```


<!-- Code of conduct -->

<div>
<h2><img src = "https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Hand%20gestures/Handshake.png" width="35" height="35"> Code of Conduct</h2>
</div>

Please note that this project is released with a [Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.


<div>
  <h2><img src="https://github.com/Meetjain1/wanderlust/assets/133582566/90f3930e-5a12-4a4e-8ac9-0dc7d5396adb" width="35" height="35">Are Ready to Contribute?</h2>
</div>

If you would like to contribute to the project then kindly go through [Contributing Guidelines](CONTRIBUTING.md) to understand everything from setup to necessary instructions.

<hr>
<h2 align = "center">Our Contributors ❤️</h2>
<div align = "center">
 <h3>Thank you for contributing to our repository</h3>

<p><a href="https://github.com/gdgmit/AgriTech-AI/contributors">
  <img src="https://contributors-img.web.app/image?repo=gdgmit/AgriTech-AI" />
  
</a></p>

</div>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## Stargazers ❤️

<div align='left'>

[![Stargazers repo roster for @gdgmit/AgriTech-AI](https://reporoster.com/stars/dark/gdgmit/AgriTech-AI)](https://github.com/gdgmit/AgriTech-AI/stargazers)


</div>

## Forkers ❤️

[![Forkers repo roster for @gdgmit/AgriTech-AI](https://reporoster.com/forks/dark/gdgmit/AgriTech-AI)](https://github.com/gdgmit/AgriTech-AI/network/members)


![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)



<!-- License -->
<div>
<h2><img src = "https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Page%20with%20Curl.png" width="35" height="35"> License:</h2>
</div>

This project is licensed under the MIT License. See the [LICENSE](https://github.com/gdgmit/AgriTech-AI/blob/main/LICENSE) file for more details.

<hr>
<div>
  Don't forget to leave a star<img src="https://fonts.gstatic.com/s/e/notoemoji/latest/1f31f/512.webp" width="35" height="30"> for this project!
</div> <br>

<a href="#top" style="position: fixed; bottom: 20px; right: 20px; background-color: black ; color: white; padding: 10px 20px; text-align: center; text-decoration: none; display: inline-block; border-radius: 5px; font-family: Arial; font-size: 16px;">Go to Top</a>
