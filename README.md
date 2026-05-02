## ML Model Deployment with BentoML (ML Zoomcamp)

This project is part of the Machine Learning Zoomcamp by DataTalksClub.

It demonstrates how to package and deploy a machine learning model as a production-ready API using BentoML.

##  Project Overview

The goal of this project is to:

* Train a machine learning model
* Package the model using BentoML
* Serve it as an API for real-time predictions

## Tech Stack

* Python
* BentoML
* Scikit-learn 
* Docker (optional)
* REST API

## Workflow

``
Data → Model Training → BentoML Packaging → API Service → Predictions

## How to Run

### 1. Install dependencies

``bash
pip install bentoml scikit-learn numpy

### 2. Train the model

```bash
python train.py
```

### 3. Serve the model

```bash
bentoml serve service:svc
```
### 4. Make a prediction

Example request:

```bash
curl -X POST http://localhost:3000/predict \
  -H "Content-Type: application/json" \
  -d '{"input": ... }'
```
### Use Cases

* Deploying ML models as APIs
* Real-time inference
* Building production-ready ML systems

### Learning Outcomes

Through this project I learned:

* How to deploy ML models using BentoML
* Packaging models for production
* Creating REST APIs for inference
* Basics of MLOps workflows

### Acknowledgments

This project is based on the Machine Learning Zoomcamp by DataTalksClub:
https://github.com/DataTalksClub/machine-learning-zoomcamp

