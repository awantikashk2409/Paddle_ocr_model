🚗 License Plate Detection & Recognition using PaddleOCR (v5 & v4)

  This project implements an end-to-end pipeline for car license plate recognition using PaddleOCR.
  The main objective was to understand how PPOCR models work in real training scenarios and to compare the performance of PPOCR v5 and PPOCR v4 on a custom license plate      dataset.

The project is divided into two complete Google Colab notebooks — one for training and one for inference — and both run fully from start to finish.

📌 Project Objective

The goal of this assignment was not just to run inference using a pretrained model, but to:

Prepare a custom dataset

Train recognition models properly

Evaluate performance

Export trained models

Compare different PPOCR versions

Visualize and analyze results

This helped in understanding the full OCR workflow — from raw images to final recognized text output.

📸 Dataset Preparation

A dataset of 100+ car license plate images was collected manually from public sources.
The dataset was formatted according to PaddleOCR recognition requirements.

The data was split as:

80% for training

20% for validation

Special attention was given to:

Clear and readable license plates

Variation in lighting conditions

Different plate formats

Slight blur and real-world distortions

This helped make the training process more realistic and practical.

📓 Notebook 1 – Training Pipeline

The training notebook includes the complete model training workflow:

Installing PaddleOCR and required dependencies

Preparing and verifying dataset format

Downloading pretrained PPOCR v5 and PPOCR v4 recognition models

Training both models separately on the custom dataset

Monitoring training loss and accuracy

Evaluating models on validation data

Exporting trained models for inference use

During training, metrics such as loss and accuracy were tracked to observe convergence and model stability.

🔍 Notebook 2 – Inference Pipeline

The inference notebook demonstrates how the trained models perform on unseen images.

It includes:

Loading exported inference models

Running recognition on test images

Displaying images with bounding boxes

Showing recognized text along with confidence scores

Side-by-side comparison between PPOCR v5 and PPOCR v4

Batch processing multiple images

Basic error analysis to identify common failure cases

Visualization makes it easy to clearly compare prediction quality between the two versions.

📊 Model Comparison & Observations

After experimentation:

PPOCR v5 showed slightly better recognition accuracy.

v5 handled noisy or slightly blurred images more effectively.

PPOCR v4 performed well but was slightly less consistent on difficult samples.

Training stability was improved in v5.

Overall, PPOCR v5 demonstrated better generalization on the validation dataset.

🚀 How to Run
Training

Open the training notebook in Google Colab and run all cells sequentially.
The model will train and export automatically.

Inference

Open the inference notebook, load the exported models, and run inference cells to view annotated results.

🧠 Key Learnings

Understanding PaddleOCR training configuration

Recognition model fine-tuning process

Model export workflow

Differences between PPOCR v4 and v5

Importance of dataset quality in OCR tasks

Practical deployment workflow from training to inference

👨‍💻 Author

Awantika Srivastava
AI/ML Engineer
