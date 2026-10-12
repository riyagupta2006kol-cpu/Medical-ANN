# Medical ANN Classifier with Zero-Knowledge Machine Learning (zkML)

## Overview

This project combines an Artificial Neural Network (ANN) with Zero-Knowledge Machine Learning (zkML) to demonstrate how medical predictions can be verified cryptographically.

The model is trained to classify diabetes outcomes using medical data. The trained neural network is exported to ONNX format and integrated with the EZKL framework to generate and verify zero-knowledge proofs for model inference.

## Objectives

- Develop an ANN model for diabetes classification.
- Train and evaluate the model using medical data.
- Export the trained model to ONNX format.
- Integrate the model with EZKL for zero-knowledge proof generation.
- Verify predictions through cryptographic proof verification.
- Demonstrate a privacy-oriented approach to verifiable machine learning.

## Dataset

This project uses the **Pima Indians Diabetes Dataset**, a benchmark dataset for binary diabetes classification.

The dataset contains eight input features:

- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- Body Mass Index (BMI)
- Diabetes Pedigree Function (DPF)
- Age

The target variable is `Outcome`, where `0` represents a non-diabetic classification and `1` represents a diabetic classification.

## Technologies Used

- **Python** — Core programming language
- **Google Colab** — Development environment
- **PyTorch** — Neural network implementation and training
- **Pandas and NumPy** — Data handling and numerical operations
- **Scikit-learn** — Data preprocessing and model evaluation
- **ONNX** — Neural network model export
- **EZKL** — Zero-Knowledge Machine Learning pipeline

## Project Workflow

1. Load and preprocess the medical dataset.
2. Split the dataset into training and testing sets.
3. Scale the input features using `StandardScaler`.
4. Build and train the Artificial Neural Network.
5. Evaluate the model using classification metrics.
6. Export the trained ANN to ONNX format.
7. Configure and compile the model using EZKL.
8. Generate a witness and cryptographic proof for inference.
9. Verify the generated proof.
10. Test proof generation and verification on additional samples.

## How to Run the Project

1. Open `Medical_ANN.ipynb` in Google Colab.
2. Run the notebook cells in sequence.
3. Allow the required Python libraries to install.
4. Ensure the dataset can be accessed.
5. Execute the ANN training and evaluation steps.
6. Run the ONNX export and EZKL proof-generation steps.
7. Review the prediction and proof-verification outputs.

The notebook generates intermediate files such as the ONNX model, configuration settings, witness, proving key, verification key, and proof.

## Expected Outcome

The project demonstrates a workflow in which a trained ANN produces diabetes classifications and EZKL is used to generate and verify cryptographic proofs of inference.

Actual model accuracy and proof-verification results should be taken from the notebook execution outputs.

## Future Scope

- Improve model performance through further experimentation.
- Explore additional medical datasets and classification tasks.
- Optimize proof-generation and verification time.
- Investigate applications of verifiable machine learning in privacy-sensitive environments.

## Disclaimer

This project is an educational and experimental implementation. It is not a clinically validated diagnostic system and should not be used to make medical decisions.

## Author

**Riya Gupta**

