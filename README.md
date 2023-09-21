# Text2Personality
# Project Proposal: Analyzing MBTI through Language

## Project Team
- [Fatemeh Ghaffarpour](mailto:fatemeh.ghaffarpour@ucalgary.ca)
- [Alireza Esmaeili](mailto:alireza.esmaeili1@ucalgary.ca)

## Problem Statement
The Myers Briggs Type Indicator (MBTI) is a widely used personality test that categorizes individuals into 16 distinct personality types based on four axes: Introversion/Extroversion, Intuition/Sensing, Thinking/Feeling, and Judging/Perceiving. Despite its popularity, the validity of MBTI has been questioned due to issues with its reliability in experiments. This project aims to investigate whether specific personality types exhibit distinct language styles and behaviors in online written content, ultimately addressing the question of the test's ability to predict and categorize behavior.

## Objectives:
The primary objectives of this project are as follows:

1. Develop and compare multiple machine learning models for predicting MBTI personality types based on text data.
2. Create a user-friendly application for predicting MBTI personality types from input text and evaluate its performance against the developed models.
3. Provide an API service that allows B2B companies to access the MBTI personality prediction functionality for employee assessments and hiring processes.

## Scope
### Model Development and Comparison:

Develop multiple machine learning models for predicting MBTI personality types from text data. These models may include natural language processing (NLP) techniques such as text preprocessing, feature extraction, and classification algorithms.
Compare the performance of these models using relevant evaluation metrics, such as accuracy, precision, recall, and F1-score.
Implement a web-based interface for users to interact with these models and input text for MBTI personality prediction.
### API Development

Build an API that exposes the MBTI personality prediction functionality to B2B companies.
### Data Analysis

Analyze the provided dataset containing over 8,600 individuals' MBTI types and their last 50 forum posts.
Extract meaningful insights regarding the relationship between language style, content, and MBTI personality types.
Visualize and present the findings in a clear and informative manner.
### User Interface (UI)

Design a user-friendly web-based interface for individuals to input text and receive MBTI personality predictions.
### Limitations

The accuracy of MBTI personality prediction models may be affected by the quality and quantity of training data and the inherent limitations of the MBTI framework.
The analysis of language style and personality may not capture the full complexity of individual personality traits.
The project's scope may be constrained by available resources, including computational power and access to data.

## Data
We will use the PersonalityCafe forum dataset, which contains MBTI types and corresponding text posts. The dataset includes information about the personality type and the last 50 posts of each individual, with posts.

## Machine Learning Models
We plan to use natural language processing (NLP) techniques and machine learning algorithms such as:
- Text preprocessing techniques (e.g., tokenization, stemming, and stop-word removal).
- Feature extraction methods like TF-IDF (Term Frequency-Inverse Document Frequency).
- Classification algorithms, including Naive Bayes, Random Forest, and deep learning models like LSTM and BERT.

The choice of models will depend on the performance and suitability for the specific problem.

## Software/hardware Architecture
Our project architecture comprises two microservices:

- ** Machine Learning Microservice:** This microservice handles the machine learning processes, including the prediction of MBTI personality types based on user-provided text.

- ** API Gateway Microservice:** This microservice serves as the entry point for external interactions. It facilitates seamless communication with our prediction models and user interface.

To ensure efficient communication between these microservices, we will implement AWS Simple Notification Service (SNS) topics and Simple Queue Service (SQS) queues within the AWS ecosystem. These components will enable streamlined data exchange and enhance the overall system's performance and reliability.

## User Interface (UI)
We will design and develop a comprehensive user interface to provide an engaging and informative user experience. Users will have the ability to:
- Input a paragraph of text for personality analysis.
- Choose one or multiple predictive models to run on their input.
- Receive a detailed report based on the selected models, allowing for result comparison.

In addition, we will implement an admin portal that offers the following features:

- Access to user-submitted records and their corresponding analysis results.
- User management capabilities for efficient administration and oversight of the platform.

## Project Timeline
- Data collection and preprocessing: Weeks 1-2
- Model development and training: Weeks 3-6
- User interface development: Weeks 7-8
- Model evaluation and fine-tuning: Weeks 9-10
- Final testing and documentation: Weeks 11-12

## Resources
- Python for data analysis and machine learning.
- Machine learning frameworks (e.g., scikit-learn and TensorFlow).
- ReactJS for the user interface development.
- Node.js for API development, catering to B2B customers, and integration with the UI.
- AWS EC2 Linux Server for deploying APIs and processing.

## Ethical Considerations
We will ensure ethical data handling, respecting user privacy, and maintaining transparency in our approach. The data used will be anonymized and stripped of any personally identifiable information.

---

**Project Repository:** [Link to GitHub Repository](https://github.com/esnf619-fall-2023/text2personality)

**GitHub Repository Description:**  
Explore the correlations between Myers Briggs Type Indicator (MBTI) personality types and language styles in online content. This repository contains the code and resources for a machine learning project that aims to predict MBTI types based on text data, evaluate the validity of the MBTI test, and provide insights into the relationship between language and personality traits. Join us in uncovering fascinating patterns in human behavior through natural language processing and data analysis.