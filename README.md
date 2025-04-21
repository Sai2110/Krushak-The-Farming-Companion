# Krushak - Sustainable Fertilizer Usage Optimizer for Higher Yield

**Krushak** is a web application that provides fertilizer recommendations to farmers based on soil reports. It leverages machine learning models to analyze soil test results (such as temperature, humidity, moisture, and nutrient content) and offers optimized fertilizer suggestions to improve agricultural yield sustainably.

## Features

- Analyzes soil reports using machine learning models
- Provides fertilizer recommendations based on soil conditions
- Easy-to-use interface for farmers to input soil data
- Built with Python, Flask, and React

## Tech Stack

- **Backend**: Python, Flask (for API)
- **Machine Learning**: Scikit-learn
- **Frontend**: React
- **Database**: MySQL (or your choice of DB)
- **Model**: Decision Tree Classifier, Naive Bayes, SVM, Logistic Regression, Random Forest
- **Deployment**: Heroku/AWS (or your preferred platform)

## Installation & Setup

### Prerequisites

Make sure you have the following installed:

- Python 3.9+
- pip (Python package installer)
- Git (optional, if using version control)

### Steps to Run Locally

1. **Clone the repository** (if using Git):

   ```bash
   git clone https://github.com/yourusername/krushak.git
   cd krushak
   ```

2. **Create and activate the virtual environment**:

   ```bash
   python -m venv py39_env
   .\py39_env\Scripts\activate   # Windows
   source py39_env/bin/activate  # Linux/Mac
   ```

3. **Install the required dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the application**:

   ```bash
   python main.py
   ```

   This will start the application on a local server, typically accessible at `http://127.0.0.1:5000/` (for Flask).

5. **Access the application** in your browser:
   Open your browser and go to `http://127.0.0.1:5000/` to see the app in action.

## Model Training

1. **Train the model** (if needed):
   The model is stored as `classifier.pkl`. If you need to retrain it, you can use the `train_model.ipynb` script to train the machine learning models and save them as a pickle file.

   Run the script by:

   ```bash
   jupyter notebook train_model.ipynb
   ```

2. **Pickle the trained model**:
   Once training is complete, save the model as:
   ```python
   import pickle
   with open('classifier.pkl', 'wb') as f:
       pickle.dump(model, f)
   ```

## File Structure
