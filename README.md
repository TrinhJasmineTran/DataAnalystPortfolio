# TRINH (JASMINE) TRAN - Business Data Analyst Portfolio
## About

Hello everyone, welcome to my portfolio! 

This is Trinh (Jasmine) and I'm a recent graduate from St. Olaf College with a BA degree in Quantitative Economics and concentrations in Data Science and Management Studies. I'm a strategic and data-driven business data analyst who loves to use data to generate key insights that drive growth and customer engagement. 

During my undergraduate time, I have developed a strong analytical and technical background in business management, marketing, and data science. I have expertise in R, SQL, Excel, Tableau, and other creative tools such as Canva and Adobe. I had opportunities to deal with large datasets, do data wrangling and transformation, and statistical modelling analysis to identify underlying patterns and trends. Also, I gained decent experience in creating insightful visualizations and preparing reports to communicate my work with various stakeholders. I strongly believe that my undergraduate experience builds a good foundation for me to further improve myself as a business data analyst.

This is a repository where I showcase my skills, projects, and keep track of my learning progress in learning Business Analysis. I'm always open to new opportunities and feedback/discussion so please feel free to reach me at tranlequetrinh2724@gmail.com.

For more information, please check out my CV here.

## Table of Contents
- [About](https://github.com/TrinhJasmineTran/DataAnalystPortfolio/edit/main/README.md#about)
- [Portfolio Projects](https://github.com/TrinhJasmineTran/DataAnalystPortfolio/edit/main/README.md#portfolio-projects)
  - SQL
    - [Career Track Analysis](https://github.com/TrinhJasmineTran/DataAnalystPortfolio/blob/main/README.md#career-track-analysis)
  - R
    - [Coffee Quality Prediction](https://github.com/TrinhJasmineTran/DataAnalystPortfolio/blob/main/README.md#coffee-quality-prediction)
    - [Handwritten Digit Recognition Using Machine Learning Algorithms]
    - [An Analysis of Key Risk Factors of Coronary Heart Disease]
    - [Sephora Skincare Analysis]
  - Tableau
    - [Car Dougscore Analysis](https://public.tableau.com/app/profile/jasmine.tran8566/viz/RevisedJasmineMM1Cars/Dashboard1)
    - [Crime In Chicago 2012-2023](https://public.tableau.com/app/profile/jasmine.tran8566/viz/RevisedJasmineMM5ChicagoCrime/Dashboard1)
    - [Tomato & Potato Production](https://public.tableau.com/app/profile/jasmine.tran8566/viz/RevisedJasmineMM3TomatoPotato/Dashboard1)
    - [AirBnb Landscape In Los Angeles](https://public.tableau.com/app/profile/jasmine.tran8566/viz/JasminesLA/Dashboard1)
    - [Minimum Wage In The US](https://public.tableau.com/app/profile/jasmine.tran8566/viz/RevisedJasmineMM4MinimumWage/Dashboard1)

- [Certificates](https://github.com/TrinhJasmineTran/DataAnalystPortfolio/blob/main/README.md#certificates)

## Portfolio projects
### Career Track Analysis

**Code:**

**Goal:**

**Description:**

**Skills:**

**Technology:**

**Results:**

### Coffee Quality Prediction

**Code:** [HTML RPubs](http://rpubs.com/trinhjasminetran27/1223031)

**Data Source:** [TidyTuesday](https://github.com/rfordatascience/tidytuesday/tree/master/data/2020/2020-07-07)

**Description and Summary:** The project aims to predict which characteristics determine the quality of coffee beans based on 4 machine learning models built on a public dataset of 1339 beans from the Coffee Quality Institute's review in January 2018. Some characteristics are aroma, acidity, aftertaste, continent of origin, species, uniformity. Comparison between models was made to identify similarities and differences of each, then uncover the most important indicators of coffee quality.

- ***Data Manipulation:*** I tidied, summarized, and modified raw data to eliminate irrelevant variables, null values, and multicollinearity. Then, divided the data into training (70%) and testing (30%) datasets.

- ***Explanatory Data Analysis:*** I created histograms and scatterplot to discover the distribution of coffee grade and the correlation between numeric variables.

- ***K-Nearest Neighbors Regression:*** using the optimal number of neighbors (17) to predict the grade of a particular bean in the data, 87% of the variability of bean quality is explained by this model.

- ***Random Forest:*** 93% of the variability of bean quality is explained by this model with 100 trees and 7 important variables.

- ***Ridge Regression:*** with the optimal penalty of only 0.001, this model explains 95.4% of the variability of coffee quality.

- ***LASSO Regression:*** this model explains the coffee grade even better, at 95.6% with 0.0183 optimal penalty.

![Coffee Results](https://github.com/user-attachments/assets/e0da691e-4599-4f04-9f3e-644971e59602)

**Skills:** data cleaning, EDA, data visualization, machine learning modelling (K-Nearest Neighbors, Random Forest, Ridge Regression with Cross-Validation, LASSO Regression with Cross-Validation), model interpretation

**Technology:** R (tidyverse, ggplot2, tidymodels, dplyr)

**Application:** Helps farmers and consumers to align expectations with each other and from that, establish a fair pricing system to ensure fair trade in the market. Informs farmers of how their product is valued and what characteristic(s) can be improved, making positive changes to their growing process and livelihood.

### Handwritten Digit Recognition Using Machine Learning Algorithms

**Code:** [Report in PDF](https://github.com/TrinhJasmineTran/DataAnalystPortfolio/blob/da1d5bb25f32eceeef94f8379381413821bcbe27/Challenge_1_Official_341.pdf)

**Description and Summary:** The project focuses on creating an end-to-end classifier of handwritten 7s and 3s by constructing two potential features and tested them on the digits of the Modified National Institute of Standards and Technology (MNIST) database. 

- ***Left Center Border:*** go through columns 14, 15, and 16 of the corresponding matrix, store the ROW number of the first non-zero cell in each column, then take the average of the three row numbers. Note that the matrix must be rotated 90 degree counterclockwise to have the corresponding image.

![Screenshot 2024-04-26 at 15_49_08](https://github.com/user-attachments/assets/21de3460-3931-4f5b-bf6c-b7f56d87ead6)

- ***Total Lower Right Quadrant Darkness:*** go through each row and column of this quadrant and sum the pixel value for each cell. Note the the matrix must be rotated 90 degree counterclockwise to have the corresponding image. 

![Screenshot 2024-04-26 at 15_41_54](https://github.com/user-attachments/assets/d2d50c4f-4ec0-4834-94cd-8143a274afdf)

- ***Dataset Creation:*** We pulled all the matrices of 3s and 7s from the MNIST dataset, calculated each feature for each matrix, and divided them into training and testing dataset at random (80/20).

- ***K-Nearest Neighbor Model:*** We built a knn model at an optimal k = 77 to get the misclassification rate of 40.5%.

- ***Logistic Regression:*** We obtained the misclassification rate of 39%

- ***Digit Visualization:*** I incorporated the rate of 39% into the classification problem and investigated the missclassified digits using visualizations.

**Skills:** machine learning algorithms and modelling, data visualization

**Technology:** R (functions, ggplot2, tidymodels)

**Application:** Assists with data entry, bank check processing, and mail sorting that contain handwritten digits. Other fields of application can be retail and logistics (invoices, forms) and education (lecture notes, materials). 

### An Analysis of Key Risk Factors of Coronary Heart Disease

**Code:** [`Coronary Heart Disease.ipynb`](https://github.com/TrinhJasmineTran/DataAnalystPortfolio/blob/c350552e8d08eb10d0589b42c7ae61d236284731/Coronary%20Heart%20Disease.ipynb)

**Report:** [PDF](https://github.com/TrinhJasmineTran/DataAnalystPortfolio/blob/c4ba327397f9c15c0d069477ec1dbf98ae10b3b5/Final_Project_Report_272.pdf)

**Description and Summary:** To investigate what factor(s) determine the development of coronary heart disease on residents of the town of Framingham, Massachusetts, our team of 2 conducted explanatory data analysis and built 4 statistical models to find the most influential variable(s) of patients. 
Some of potential risk factors are age, gender, educational level, smoker/non-smoker, if a patient takes blood pressure medications, prevalance of stroke, obesity, heart rate, etc.

- ***Explanatory Data Analysis:*** I plotted the relationship between the binary response variables with each of the explanatory variables to investigate correlation. A segmented bar chart and table of proportions were used for categorical variables, while continuous quantitative variables were observed using histograms.
- ***Logistic Regression:*** To make comparisons between groups (binary variables), we employed simple and multiple logistic regression.
- ***LASSO Variable Selection:*** we run the selection to eliminate weak indicators of heart disease in the data.

**Skills:** data preprocessing, data analysis, statistical modelling (linear regression, logistic regression, LASSO Model Selection), statistical writting

**Technology:** R (tidyverse, dyplyr, ggplot2)

**Application:** Uncovers the relationship between conary heart disease with several risk factors, helping patients and researchers in studying this disease.

### Sephora Skincare Analysis

**Code:** [`Sephora Skincare Analysis.ipynb`](https://github.com/TrinhJasmineTran/DataAnalystPortfolio/blob/9a9c3ca33e210abff68e301dbfd90fae4fc045d1/Sephora%20Skincare%20Analysis.ipynb)

**Description and Summary:** With a love for beauty products, my team of 2 decided to make an interactive webpage using RShiny to study Sephora’s portfolio of brands and products. We focused on categorizing brands into cruelty-free and non-cruelty-free and from that, allowed users to choose products according to their willingness to purchase, choices of brands, skin types, and skin conditions. Our webpage has 6 tabs with drop-down menus for better user interaction.

- ***Data Preparation:*** We found two datasets (product data and cruelty-free data) related to the topic and joined them to have a master dataset. We tidied and wrangled the 3 datasets (2 original and a master one) using join and pivot functions in RStudio.

- ***Visualization Sketching:*** Pre-coding, we sketched some visualization ideas on paper to make sure the axes, variables, and graph structures work well. This step also stimulated the creativity for better ideas. 

- ***Coding & Data Visualization:*** I first learned how to code a webpage by going though online tutorials and resources from the Professor. It’s worth paying attention to coding the page structure, layout, images, and titles. Then, we dived into making the visualizations and interactive parts like drop-down menus and bars.

**Skills:** Data preprossing, analysis, and visualization

**Technology:** R (tidyverse, ggplot2, dyplyr, RShiny)

**Application:** Gains awareness for consumers of the beauty industry to study the brands and products more carefully, according to their demands and skin types.
Helps avoid wasting of resources as beauty products can be a magic for someone while being a nightmare for someone else. 

## Certificates
- [The Complete SQL Bootcamp: From Zero To Hero (Jun 2024)](https://github.com/TrinhJasmineTran/DataAnalystPortfolio/blob/6bb3cb7720d853d93f39c9d121543978b3512016/UC-4d30e5ac-ba35-4d71-9f43-a1bde5e197ca.jpg)  | Udemy
- [Learning SQL Programming (Jan 2024)](https://github.com/TrinhJasmineTran/DataAnalystPortfolio/blob/27f48ebe202aadeb59987cd109a809c88c51a1fb/CertificateOfCompletion_Learning%20SQL%20Programming.pdf)  | LinkedIn Learning


