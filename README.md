# Student Performance Prediction System

## Overview

This project is a web-based Student Performance Prediction System that leverages machine learning to forecast a student's potential academic outcome (final grade range) and identify those who might be at academic risk. By analyzing various input features related to a student's academic journey, the system aims to provide valuable insights for students, educators, and academic advisors, enabling proactive interventions and personalized support.

## Features

* **User-Friendly Interface:** Students can easily input their academic information through a web browser.
* **Dynamic Input:** Allows adding multiple courses and certificates.
* **Comprehensive Data Collection:** Gathers information on course grades and credits, attendance, CGPA, internships, and certificates.
* **AI-Powered Predictions:** Utilizes trained machine learning models (Random Forest and Logistic Regression) to predict the final grade range and academic risk level.
* **Personalized Recommendations:** Provides tailored advice based on the predicted outcomes and input data.
* **Clear Results Display:** Presents the predictions and recommendations in an easy-to-understand format.

## Technologies Used

* **Frontend:** HTML, CSS, JavaScript
* **Backend:** Python (Flask)
* **Machine Learning:** scikit-learn (Random Forest, Logistic Regression, StandardScaler), pickle
* **Automation:** Bash (for running the application)

## Setup and Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Bharath72997/student-performance-prediction-system]
    cd [repository name]
    ```

2.  **Ensure Python is installed:** This project requires Python 3.

3.  **Install the required Python libraries:**
    ```bash
    pip install -r requirements.txt
    ```
    *(Note: You might need to create a `requirements.txt` file listing dependencies like Flask, scikit-learn, pandas, numpy, and flask-cors if you haven't already.)*

4.  **Run the application:**
    ```bash
    chmod +x run.sh
    ./run.sh
    ```
    This script will:
    * Create the `models` directory if it doesn't exist.
    * Train the machine learning models using synthetic data (if the model files are not already present).
    * Start the Flask development server.

5.  **Access the application:** Open your web browser and navigate to `http://127.0.0.1:5000/`.

## Usage

1.  Open the web application in your browser.
2.  Enter the student's academic information in the provided form, including course grades and credits, attendance, CGPA, internship details, and certificates.
3.  Click the "My Performance" button.
4.  The system will send the data to the backend for prediction.
5.  The results, including the predicted final grade range, risk level, and personalized recommendations, will be displayed on the page.

## Machine Learning Models

This project utilizes the following machine learning models:

* **Random Forest Classifier:** Used for predicting the student's final grade range based on the input features.
* **Logistic Regression:** Used for predicting the student's academic risk level (e.g., low, moderate, high).
* **StandardScaler:** Used for feature scaling to standardize the input data before feeding it to the models.

The models are trained using the `train_models.py` script (currently with synthetic data for demonstration purposes) and saved in the `models/` directory.

## Future Work

* Train the models on a larger, real-world dataset for improved accuracy and generalization.
* Implement user authentication and data storage.
* Add more sophisticated features and recommendations.
* Explore other machine learning models for potential performance gains.
* Integrate with existing learning management systems (LMS).
* Provide more detailed feedback and explanations for the predictions.
* Develop visualizations of student performance trends.

## Contributing

Contributions to this project are welcome. Please feel free to submit pull requests or open issues for any bugs or feature requests.

## AUTHOR

Bharath Chandra
