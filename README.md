# DishWise

DishWise is a platform that empowers college students in food entrepreneurship by providing AI-driven insights for ingredient cost management and optimal purchasing strategies.

## Problem

College students face challenges in determining investment and menu pricing due to fluctuating ingredient costs and limited real-time data, leading to financial miscalculations.

## Solution

Using an AI model, DishWise predicts ingredient prices based on district, commodity, and time, and suggests the best buying month and nearby districts with lower costs to improve financial planning.

## How do we solve the problem?

### Data Collection

For the DishWise price prediction model, the preprocessing involved several key steps to prepare the dataset. The commodity price data was merged with seasonal information to enrich the dataset. The 'Arrival_Date' column was converted to a datetime format, and the year and month were extracted for better analysis. Additionally, the dataset was sorted by district, market, commodity, and variety. To ensure accurate month representation, numerical month values were mapped to their corresponding names. For large data handling, the dataset was split into manageable chunks to optimize processing. This preprocessed data will be used for further prediction and model training.

### Selecting Pre-trained Model

For the DishWise project, we employed the RandomForestRegressor as our primary machine-learning model. Random Forest is an ensemble model that constructs multiple decision trees and averages their predictions to improve accuracy and reduce overfitting. To enhance performance, we used RandomizedSearchCV to fine-tune the model’s hyperparameters such as the number of estimators, maximum tree depth, and minimum samples required at each split. This approach allows us to efficiently optimize the model and achieve more accurate price predictions for various commodities across districts and timeframes.

## How do we present it?

To make our model user-friendly, we developed an attractive web application that allows users to easily input parameters such as district, commodity, variety, year, and month for price predictions. Using HTML, CSS, and JavaScript, we integrated it with Flask for backend processing. The app features a main page for input and a results page for displaying predictions, ensuring a seamless user experience. This engaging interface makes it accessible for users of all technical backgrounds to utilize the price prediction model effectively.
![App Screenshot]("G:\DishWise-main\DISHWISE\DishWise-main\static\images\Screenshot 2024-10-05 100027.png")
## Technologies Used

We utilized a diverse set of technologies, which can be categorized into three parts:

### Frontend:
- *JavaScript*: The dynamic framework of choice for an engaging user experience.
- *HTML*: The structure for our visually appealing interface.
- *CSS*: Styling that brings a modern touch to our application.

### Backend:
- *Flask*: The powerful web framework that showcases the versatility of Python.

### Machine Learning:
- *Scikit-learn*: The backbone of our machine learning operations.
- *RandomForestRegressor*: The algorithm used for accurate price predictions.
- *RandomizedSearchCV*: A tool for optimizing hyperparameters effectively.
- *OneAPI*: The star technology that enhances performance and scalability.

## Why did we choose OneAPI?

OneAPI is a powerful tool for machine learning projects that can help developers achieve better performance and code portability. With its optimized libraries, performance tools, and unified programming model, OneAPI can speed up training and improve inference performance. It also simplifies development by enabling developers to write code that can run on different hardware platforms.

### Its key benefits include:
- *Accelerating training* on hardware accelerators like GPUs or FPGAs.
- *Improving inference performance* on various hardware platforms, which can reduce latency and improve throughput.
- *Increasing code portability* by enabling developers to write code that can run on different hardware architectures.
- *Optimizing performance* with performance tools that can help developers improve the performance of their code.
- *Simplifying development* with a unified programming model that can help reduce the need for platform-specific code.

### Benchmarks

Using OneAPI in our project gave us an ultimate uplift in timetaken. This may seem like a tiny improvement, but on larger datasets, this will impact accuracy on a larger scale.

Note: These benchmarks are taken on machines with identical specs

# WEBSITE
![Screenshot 2024-10-05 100027](https://github.com/user-attachments/assets/0ebf098b-3c2f-4015-8a54-acf0672374c6)
![Screenshot 2024-10-05 100920](https://github.com/user-attachments/assets/bcb75b8e-1ac2-40ba-a615-83411dfa17c2)
![Screenshot 2024-10-05 100928](https://github.com/user-attachments/assets/bfb8b50c-da84-4a3a-a6f4-0af3c5e16931)

# IN INTEL ONE API JUPYTER NOTEBOOK
![Screenshot 2024-10-13 085157](https://github.com/user-attachments/assets/039a51c4-92f4-4884-9f42-4369da5f6acd)

# IN LOCAL MACHINE
![Screenshot 2024-10-13 091107](https://github.com/user-attachments/assets/1925bba9-0e27-4280-8319-28b45f9ddbeb)
