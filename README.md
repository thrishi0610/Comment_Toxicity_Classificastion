**TOXIC COMMENT CLASSIFIER**

This project is a deep learning-based application for classifying user-generated comments as toxic or non-toxic. It leverages a simple neural network architecture, built using TensorFlow, and is deployed with an interactive Gradio interface. The entire pipeline, from data preprocessing to deployment, is implemented in Google Colab.

**OVERVIEW**

The goal of this project is to identify toxic behavior in online comments. Using the Jigsaw Toxic Comment Classification dataset, the model is trained to detect whether a comment contains toxicity, and then deployed with a minimal UI for real-time testing.

**FEATURES**

1) Text preprocessing and tokenization

2) Neural network model for binary classification

3) TensorFlow implementation with GPU acceleration (Colab)

4) Gradio interface for live testing

5) Ready-to-use in Google Colab

6) Project Structure
  sql
  Copy
  Edit
  Toxic-Comment-Classifier/
  ├── README.md
  ├── ToxicClassifier.ipynb
  ├── data_given/
  │   └── train.csv
  └── requirements.txt

**DATASET**

The project uses the publicly available Jigsaw Toxic Comment Classification dataset, which contains thousands of comments labeled for various types of toxicity such as:

toxic

severe_toxic

obscene

threat

insult

identity_hate

**Dataset Source:**
Kaggle - Jigsaw Toxic Comment Classification Challenge

**Model Architecture**

Embedding Layer

GlobalAveragePooling1D Layer

Dense Output Layer with Sigmoid Activation

Loss Function: Binary Crossentropy
Optimizer: Adam
Evaluation Metric: Accuracy

Training Environment
Google Colab with GPU enabled

TensorFlow 2.x

Pandas and Numpy for data manipulation

Gradio for interactive deployment

Running the Interface in Colab
Upload the dataset (train.csv) to your environment.

Run all the notebook cells in order.

At the end, launch the Gradio app using:

python
Copy
Edit
interface.launch(share=True)
A public URL will be generated to test the model in real-time.
