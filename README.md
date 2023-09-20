# Insurance Cross-Sell Prediction Project

![Project Image](/demo/project-demo.gif)

Welcome to the **Insurance Cross-Sell Prediction Project**, a comprehensive end-to-end AutoML solution designed to revolutionize the insurance industry. This project harnesses the power of cutting-edge technologies including H2O AutoML, MLflow, FastAPI, and Streamlit to enhance cross-selling campaigns and boost efficiency.

## Table of Contents
- [Business Overview](#business-overview)
- [Technical Insight](#technical-insight)
- [Objective](#objective)
- [Pipeline Components](#pipeline-components)
- [User Interface Demo](#user-interface-demo)
- [Project Structure](#project-structure)
- [References](#references)

## Business Overview

Cross-selling in the insurance sector is all about offering complementary products to existing policyholders. It aims to provide customers with comprehensive protection at an attractive bundled cost while helping insurers increase their revenue through enhanced policy conversions. Our project focuses on identifying health insurance customers who are likely to be interested in purchasing additional vehicle insurance, making cross-sell campaigns more efficient and targeted.

## Technical Insight

Traditionally, developing machine learning models for such tasks has been a time-consuming and resource-intensive process that demands significant technical expertise. However, with the advent of Automated Machine Learning (AutoML), the process has become streamlined and efficient. Beyond model development, there are various components in a production-ready ML system. This project demonstrates how to set up, train, and serve such a system using the following technologies:

- **H2O AutoML**: To automate the model selection and tuning process.
- **MLflow**: For tracking and managing machine learning experiments.
- **FastAPI**: To deploy the best H2O model for real-time inference.
- **Streamlit**: For creating an intuitive user interface to interact with the model.

## Objective

Our main objective is to make cross-selling more efficient and targeted by building a predictive ML pipeline. This pipeline identifies health insurance customers who are interested in purchasing additional vehicle insurance, enabling insurance companies to focus their cross-sell efforts effectively.

## Pipeline Components

1. **Data Acquisition and Preprocessing**: The foundation of any successful ML project begins with data. We prepare and preprocess our data to ensure it's ready for modeling.

2. **H2O AutoML Training with MLflow Tracking**: We leverage H2O AutoML to automatically explore and build the best machine learning model, tracking each step with MLflow.

3. **Deployment of Best H2O Model via FastAPI**: Once we have our winning model, it's deployed using FastAPI, providing a robust and efficient API for real-time predictions.

4. **Streamlit User Interface**: We create an intuitive Streamlit user interface that allows users to input data and receive predictions seamlessly.

## User Interface Demo

![UI Demo](/demo/ui-demo.gif)

## Project Structure

- **/backend**: Contains files for setting up the backend, including the H2O ML model and FastAPI instance.
- **/data**: Houses raw data, processed data, and output data in JSON format.
- **/mlruns**: Stores artifacts from ML training experiments.
- **/utils**: Contains Python scripts with helper functions.
- **main.py**: The script for selecting the best H2O model and deploying it as a FastAPI endpoint.
- **Dockerfile**: Used to build the backend service as a Docker container.
- **train.py**: The script for executing H2O AutoML training with MLflow tracking.
- **/frontend**: Contains the frontend user interface (UI) aspect of the project built using Streamlit.
- **app.py**: The script for the Streamlit web app, connected to the FastAPI endpoint for model inference.
- **Dockerfile**: Used to build the frontend service as a Docker container.
- **/demo**: Includes GIF and webm files showcasing the Streamlit UI demo.
- **/notebooks**: Contains Jupyter notebooks for EDA, XGBoost baseline, and H2O AutoML experiments.
- **submissions**: Holds CSV files for Kaggle submission to retrieve model accuracy scores.

## References

For more in-depth information, check out these valuable resources:
- [H2O AutoML Documentation](https://docs.h2o.ai/h2o/latest-stable/h2o-docs/automl.html)
- [MLflow Documentation for H2O](https://www.mlflow.org/docs/latest/python_api/mlflow.h2o.html)
- [Guide on Building a Multi-Class Classification Model in Python](https://setscholars.net/automl-h2o-project-a-guide-to-build-a-multi-class-classification-model-in-python-using-car-description-data/)
- [FastAPI Request Files Tutorial](https://fastapi.tiangolo.com/tutorial/request-files/)
- [Fundamentals of MLOps with MLflow and FastAPI](https://medium.com/analytics-vidhya/fundamentals-of-mlops-part-4-tracking-with-mlflow-deployment-with-fastapi-61614115436)
- [FastAPI and Streamlit Integration](https://testdriven.io/blog/fastapi-streamlit/)
- [Deploying Machine Learning Models with Streamlit, FastAPI, and Docker](https://rihab-feki.medium.com/deploying-machine-learning-models-with-streamlit-fastapi-and-docker-bb16bbf8eb91)
- [Streamlit FastAPI ML Serving](https://davidefiocco.github.io/streamlit-fastapi-ml-serving/)

This project aims to transform the insurance industry by making cross-selling smarter and more efficient. We hope you find it informative and inspiring for your own machine learning endeavors!
