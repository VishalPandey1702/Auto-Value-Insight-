# Car Price Prediction Application

## Overview

This project is a web-based application that allows users to submit car details and receive a predicted price for the car. It consists of a React frontend for collecting user input and a Flask backend for processing the data and making predictions using a machine learning model.

## Features

- **User Input Form:** A dynamic form in the React frontend that allows users to input details such as car name, location, fuel type, transmission, owner type, mileage, engine capacity, power, year of manufacture, kilometers driven, and number of seats.
- **Data Submission:** User inputs are sent to the Flask backend via a POST request for processing.
- **Machine Learning Model:** The Flask backend processes the data and predicts the car price using a pre-trained machine learning model.
- **Response Display:** The predicted price and a success message are displayed back to the user on the frontend.

## Technologies Used

- **Frontend:** 
  - React
  - HTML/CSS (with Tailwind CSS for styling)

- **Backend:** 
  - Flask
  - Python
  - Scikit-learn (for machine learning)


- **App.js:** React component for rendering the input form and displaying the server's response.
- **App.css:** CSS file for styling the frontend components.
- **app.py:** Flask application that handles incoming POST requests and returns the predicted price.
- **process.py:** Contains the machine learning model and prediction logic.
- **dataconversion.py:** Handles the formatting of input data before processing.
- **dataset.csv:** Dataset used for training the machine learning model.

## Setup and Installation

### Frontend (React)

1. Navigate to the `client` directory:
    ```bash
    cd client
    ```
2. Install the required dependencies:
    ```bash
    npm install
    ```
3. Start the React development server:
    ```bash
    npm start
    ```

### Backend (Flask)

1. Navigate to the `server` directory:
    ```bash
    cd server
    ```
2. Create and activate a virtual environment (optional but recommended):
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```
3. Install the required Python packages:
    ```bash
    pip install -r requirements.txt
    ```
4. Run the Flask server:
    ```bash
    python app.py
    ```

## Usage

1. Start both the React frontend and the Flask backend.
2. Open the frontend in your browser (usually at `http://localhost:3000`).
3. Fill out the car details in the form and submit.
4. View the predicted price returned from the server.

## Example Response

```json
{
  "status": "success",
  "predicted_price": 450000,
  "message": "Data received and processed successfully!"
}

![Submit Car Details](../src/app.png)

