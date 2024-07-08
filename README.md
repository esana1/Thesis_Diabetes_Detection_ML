# Machine Learning Techniques for Diabetes Detection Using Iris and Conjunctival Images

This project leverages machine learning techniques to detect diabetes using high-resolution images of the iris and conjunctiva. By analyzing these images, we aim to develop non-invasive methods for early diabetes detection and provide actionable insights for medical professionals.

## Table of Contents
- [Introduction](#introduction)
- [Global Perspective on Diabetes](#global-perspective-on-diabetes)
- [Diabetes in India](#diabetes-in-india)
- [Current Methods for Diabetes Detection](#current-methods-for-diabetes-detection)
- [Why Machine Learning?](#why-machine-learning)
- [Data](#data)
- [Methodology](#methodology)
- [Analysis](#analysis)
- [Results](#results)
- [Recommendations](#recommendations)
- [Conclusion](#conclusion)
- [How to Use](#how-to-use)
- [Contributors](#contributors)

## Introduction
Diabetes is a chronic disease characterized by elevated levels of blood glucose (or blood sugar), which can lead to serious damage to the heart, blood vessels, eyes, kidneys, and nerves over time. Early detection and management are crucial to prevent complications.

## Global Perspective on Diabetes
As of 2021, approximately 537 million adults are living with diabetes worldwide. It is one of the major causes of morbidity and mortality, significantly affecting individuals' quality of life and posing a substantial economic burden on healthcare systems globally.

## Diabetes in India
India is often referred to as the "diabetes capital of the world," with over 77 million adults diagnosed with diabetes. This number is expected to rise to 134 million by 2045. The high prevalence is attributed to genetic predisposition, lifestyle changes, and rapid urbanization. Despite the large number of cases, nearly 50% of people with diabetes remain undiagnosed, highlighting the need for improved detection methods.

## Current Methods for Diabetes Detection
### Traditional Methods
1. **Hemoglobin A1c Test (HbA1c)**: Reflects average blood sugar levels over the past two to three months.
2. **Fasting Plasma Glucose Test (FPG)**: Measures blood sugar after an overnight fast.
3. **Oral Glucose Tolerance Test (OGTT)**: Measures blood glucose before and two hours after consuming a glucose-containing beverage.
4. **Random Plasma Glucose Test**: Measures blood sugar without regard to last meal timing.
5. **Glycosuria Test**: Detects the presence of glucose in the urine.

### Non-Traditional Methods
1. **Breath Analysis**: Detects higher acetone levels in diabetic patients' breath.
2. **Saliva Testing**: Researching the correlation between saliva and blood glucose levels.
3. **Tear Analysis**: Developing devices to monitor tear glucose levels.
4. **Sweat Monitoring**: Tracks glucose levels via sweat analysis using biosensors.
5. **Spectroscopy**: Uses light waves to measure glucose levels.

## Why Machine Learning?
Machine learning (ML) offers a non-invasive, efficient, and accurate alternative for diabetes detection. The advantages include:
- **Early Detection**: ML can identify subtle patterns and early signs of diabetes that might be missed by traditional methods.
- **Automated Analysis**: Provides a fast and objective analysis of medical images.
- **Patient Comfort**: Non-invasive and painless procedures.
- **Scalability**: Can be easily integrated into telemedicine platforms for remote screening, especially in underserved areas.
- **Cost-Effectiveness**: Reduces the need for expensive and invasive diagnostic tools.

## Data
The dataset used in this project includes:
- **Iris Images**: 800 images collected from JNMCH, categorized as diabetic and non-diabetic.
- **Conjunctival Images**: 572 images collected from JNMCH, categorized as diabetic and non-diabetic.

## Methodology
### Data Preprocessing
1. **Loading Images**: Iris images are loaded in grayscale mode to reduce computational complexity.
2. **Applying Otsu's Thresholding**: This method separates the iris (assumed to be darker) from the rest of the image.
3. **Morphological Operations**: Erosions and dilations are performed to remove noise.
4. **Finding Contours**: Contours in the thresholded image are identified to locate the iris.
5. **Creating a Mask**: A mask is created to fill in the contour of the iris.
6. **Applying the Mask**: The mask is applied to the original image to isolate the iris.

### Feature Selection
Identifying key attributes in the iris and conjunctival images that influence diabetes detection.

### Model Training Pipeline
1. **Reshape Images**: Images are reshaped to a uniform size of 150x150 pixels.
2. **Encode Labels**: Labels are transformed from categorical to numerical values.
3. **Split Data**: Data is split into training and testing sets.
4. **Train, Predict, and Evaluate**: Machine learning models are trained, predictions are made, and evaluations are conducted using various metrics.

### Model Training and Evaluation
Developing and evaluating models such as:
- **Decision Trees**
- **Support Vector Machine (SVM)**
- **K-Nearest Neighbors (KNN)**
- **Random Forest**
- **Naive Bayes**
- **Gradient Boosting**

## Analysis
### Exploratory Data Analysis (EDA)
Investigating trends and patterns in the iris and conjunctival images, including:
- **Distribution of Diabetic and Non-Diabetic Images**
- **Age Distribution of Subjects**
- **Correlation between Image Features and Diabetes**

### Machine Learning Models
Analyzing the performance of various machine learning models on the datasets. 

## Results
### Iris Images
- **SVM (Poly)**: Achieved 95% accuracy
- **Random Forest**: Achieved 94% accuracy

### Conjunctival Images
- **SVM (Poly)**: Achieved 93.3% accuracy
- **Random Forest**: Achieved 93% accuracy

### Combined Iris and Conjunctival Images
- **SVM (Poly)**: Achieved 96.78% accuracy
- **Random Forest**: Achieved 94% accuracy

## Recommendations
1. **Advanced Models Exploration**: Utilize more sophisticated machine learning and deep learning models to potentially enhance results.
2. **Multi-Disease Framework**: Expand the developed framework to detect multiple diseases, including other ocular and systemic conditions.
3. **Clinical Integration**: Investigate practical implications and benefits of embedding these models in clinical practice for early detection of diabetes.
4. **Expansive Diverse Datasets**: Collect larger and more diverse datasets, capturing data from various regions, ages, and disease stages to boost the model's universality.

## Conclusion
The project demonstrates the potential of using machine learning for non-invasive diabetes detection with high accuracy. The innovative approach using iris and conjunctival images marks a significant step towards early diabetes detection, reshaping the landscape of medical diagnostics.

## How to Use
Clone the repository:
```sh
git clone https://github.com/esana1/Diabetes-Detection-Using-ML.git
```
## Contributors

- Ehtesham Sana
- Dr. Nadeem Akhtar
- Dr. Hamid Ashraf
