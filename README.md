# Cyberbullying Detection Using Machine Learning

## Overview
This project develops a machine learning-based system designed to detect cyberbullying in online platforms using advanced natural language processing (NLP) techniques and machine learning algorithms from the **sklearn** library. With the rise of social media and digital communication, this system aims to provide a scalable solution for real-time detection of harmful content, ensuring safer online spaces for users.

## Objective
The objective of this project is to build an automated content moderation system that can classify user-generated text as either **bullying** or **non-bullying** using machine learning algorithms, specifically Logistic Regression, Support Vector Machines (SVM), and Random Forest. The system uses NLP techniques for preprocessing and vectorization of text data, improving its ability to classify and predict instances of cyberbullying.

## Key Features
- **Text Preprocessing**: Tokenization, stop word removal, lemmatization, and vectorization (TF-IDF).
- **Machine Learning Algorithms**: Implementation of Logistic Regression, SVM, and Random Forest for text classification.
- **Model Evaluation**: Performance evaluated using accuracy, precision, recall, and F1-score metrics.
- **Real-Time Detection**: Scalable solution designed for real-time detection and integration into social media platforms.

## Technologies Used
- **Python**: Programming language for implementing the machine learning models and preprocessing tasks.
- **scikit-learn (sklearn)**: Library for machine learning models and tools for data mining and analysis.
- **NLTK**: Library for NLP tasks, including tokenization, stemming, and stop word removal.
- **Flask**: Framework for deploying the trained model as a web service for real-time predictions.
- **Pandas**: For data manipulation and cleaning.
- **Matplotlib**: For visualizing data and evaluating model performance.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/subramanyamrekhandar/Real-Time-Cyberbullying-Detection-Using-NLP-and-sklearn-Models.git
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## How It Works
1. **Data Collection**: User-generated text data from platforms like Twitter and YouTube are collected and labeled as bullying or non-bullying.
2. **Preprocessing**: The collected text data is cleaned using tokenization, stop word removal, and lemmatization.
3. **Model Training**: Machine learning models (Logistic Regression, SVM, Random Forest) are trained on the preprocessed data to classify text into bullying or non-bullying categories.
4. **Evaluation**: The models' performance is evaluated using metrics like accuracy, precision, recall, and F1-score.
5. **Deployment**: The model is deployed via Flask as an API, enabling real-time detection on social media platforms.

## Example Usage

To run the model and make predictions, use the Flask API as follows:

1. Start the Flask server:
    ```bash
    python app.py
    ```

2. Send a POST request with a text sample to the `/predict` endpoint:
    ```bash
    curl -X POST -d "text=Your sample text here" http://localhost:5000/predict
    ```

3. The API will return a prediction indicating whether the text is bullying or non-bullying.

## Evaluation Metrics
The system’s performance is evaluated based on:
- **Accuracy**: Proportion of correctly classified instances.
- **Precision**: Proportion of true positives among predicted positives.
- **Recall**: Proportion of true positives among actual positives.
- **F1-Score**: Harmonic mean of precision and recall, balancing both metrics.

## Future Improvements
- **Multilingual Support**: Extend the system to handle different languages and cultural contexts.
- **Deep Learning Models**: Incorporate more advanced models like LSTMs and CNNs for deeper context understanding.
- **Cross-Platform Integration**: Implement the solution across multiple platforms to detect cyberbullying on various social media sites.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- **scikit-learn** for machine learning algorithms and tools.
- **NLTK** for natural language processing support.
- **Flask** for creating a real-time deployment solution.
