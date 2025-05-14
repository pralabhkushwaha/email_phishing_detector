# Email Phishing Detector App

## Overview
This is a Streamlit application that helps detect phishing emails using machine learning. The application allows users to:
1. Classify emails as phishing or legitimate
2. Train their own phishing detection model
3. Learn about email phishing and how to avoid it

## Features
- Email classification based on content analysis
- Custom model training with user data
- Feature extraction from email content
- Interactive UI with result explanation
- Model saving and downloading

## Requirements
- Python 3.7+
- Streamlit
- Pandas
- NLTK
- Scikit-learn
- Pickle

## Installation
1. Clone this repository or download the code
2. Install the required dependencies:
```
pip install streamlit pandas nltk scikit-learn
```

## Usage
1. Navigate to the project directory
2. Run the Streamlit app:
```
streamlit run app.py
```
3. The app will open in your web browser

## How to Use
The application consists of three tabs:

### Email Classification
- Enter the email content you want to analyze
- Click "Analyze Email" to get the classification result
- View detailed analysis of the email with phishing indicators

### Model Training
- Upload your own CSV dataset with email texts and labels
- Alternatively, use the sample data provided
- Train the model and download it for future use

### About
- Learn about email phishing
- Understand how the detector works
- Get tips to avoid phishing attacks

## Data Format
When training with your own data, the CSV file should contain:
- A column named 'email_text' containing the email content
- A column named 'label' with values 1 (phishing) or 0 (legitimate)

## Performance Notes
- The model performs best with balanced datasets
- More training data generally leads to better performance
- The app uses a Random Forest classifier with TF-IDF vectorization for text features

## License
This project is for educational purposes only.
