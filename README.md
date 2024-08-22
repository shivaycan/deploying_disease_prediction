# Disease Prediction and AI Chat Application

## Overview

This project consists of a web application that predicts diseases based on symptoms using a trained machine learning model and also provides an interactive chat experience through Google Generative AI. The application is built using Flask and integrates several components to offer disease prediction and responsive chat functionalities.

## Components

### `train_model.py`

- **Purpose:** Trains a Support Vector Machine (SVM) model using a dataset (`Dataset.csv`), preprocesses the data, and saves the trained model to a file (`ML_model.pkl`).
- **Functionality:** Think of this as creating a recipe for predicting diseases based on symptoms. It handles data preparation, model training, and saving the model.

### `AI.py`

- **Purpose:** Contains functions for interacting with Google Generative AI.
- **Functionality:** Helps generate responses based on user input. This file is used by the backend to handle chat-related requests, similar to having a smart assistant that can respond to questions about symptoms and diseases.

### `main.py`

- **Purpose:** Core of the application, sets up a web server using Flask.
- **Functionality:** Defines two main functionalities:
  - **Disease Prediction:** Loads the trained model from `ML_model.pkl` and provides an endpoint where users can send their symptoms to get a disease prediction.
  - **Chat Interaction:** Uses functions from `AI.py` to handle chat requests, allowing users to ask questions and get responses related to their symptoms.

### `app.py`

- **Purpose:** Integrates the web server with the AI functionalities.
- **Functionality:** Provides endpoints for both disease prediction and chat interactions. It ensures that the web application can handle requests from users, perform predictions, and engage in conversations.

## Setup and Installation

1. **Clone the Repository:**
   ```bash
   git clone <repository-url>
   cd <repository-folder>



pip install -r requirements.txt
python train_model.py
python main.py
