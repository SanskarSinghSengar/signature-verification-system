# signature-verification-system
# AI-Powered Signature Verification System | Nyaya-Jyoti Project
Welcome to the official repository of an AI-based Signature Verification System developed for the Nyaya-Jyoti project — a legal documentation and authentication platform powered by machine learning.

🌟 Project Overview
Nyaya-Jyoti aims to bring transparency, accountability, and digital trust to legal processes by verifying handwritten signatures using deep learning. This notebook provides a Google Colab-ready implementation of a Siamese Neural Network trained on the CEDAR signature dataset, with a user-friendly interface for uploading and verifying signatures.

📌 Features
✅ Built using a Sigmoid-based Siamese Neural Network (SNN)

📦 Utilizes the CEDAR dataset of real and forged signatures

🔐 Supports multi-user signature enrollment

🧪 Allows users to upload test signatures and verify authenticity

📊 Provides confidence scores on signature similarity

🎯 Trained with advanced techniques like Early Stopping and Learning Rate Scheduling

☁️ Fully Google Colab-compatible

⚙️ How It Works
1. Signature Enrollment
You start by uploading a ZIP file containing real signature images (from the CEDAR dataset).

Then, add users one by one.

For each user, upload exactly 5 genuine signatures for the system to learn their writing style.

2. Training the Model
The system generates positive and negative signature pairs.

A Siamese Neural Network is trained to distinguish between genuine and forged pairs based on their feature distance.

Optimizations include:

EarlyStopping

ReduceLROnPlateau

Adam Optimizer

3. Signature Verification
Users can upload any new signature image.

The system compares it with every stored signature using the trained SNN.

The model outputs a confidence score (0–1) for each user.

If a score exceeds 0.5, the user is considered verified.

🧑‍💼 Use Case: Nyaya-Jyoti Platform
Nyaya-Jyoti is a legal documentation platform where signature-based verification is crucial for:

Court affidavits

E-signed agreements

Legal petitions

Will and testament submissions

This AI model strengthens digital documentation by offering real-time verification and reducing forgery.

🚀 How to Use This Notebook
👉 Recommended Environment: Google Colab

Step-by-Step Instructions:
Upload CEDAR ZIP Dataset
Run the notebook cell and drag your cedar.zip file containing real signatures.

Add Users

Enter a username (e.g., "John_Doe")

Upload exactly 5 genuine signature images for that user

Repeat for multiple users

Model Training Starts Automatically

Trains a Siamese Network on the generated positive/negative pairs

Verify New Signatures

Upload a signature image

The system compares it to all stored signatures

If a match is found, it prints the user name and confidence score

📁 Dataset Used: CEDAR
Source: CEDAR Signature Dataset

12 Users × 24 Signatures (Genuine + Forged)

Format: PNG/JPG grayscale

🛠️ Technologies Used

Tech	Role
Python	Core programming
TensorFlow / Keras	Deep learning framework
OpenCV	Image processing
Scikit-learn	Dataset splitting
Google Colab	Cloud-based execution
matplotlib	Plotting and visualization
🔒 Security & Ethical Use
This system is built for legal, educational, and ethical use only. It is meant to assist in verification, not fully replace human judgment. Data used should comply with privacy laws and user consent.

📬 Feedback & Contributions
Feel free to:

Submit pull requests

Report issues

Fork the repo and build upon it!

We welcome contributions from the AI, legal tech, and cybersecurity communities.


