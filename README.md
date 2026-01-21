
Customer Complaint Root Cause Analysis

This project utilizes Natural Language Processing (NLP) and Unsupervised Machine Learning to automatically categorize customer complaints and identify their underlying root causes. By leveraging sentence embeddings and K-Means clustering, the system can group similar issues without needing pre-labeled data.

🚀 Features
Semantic Text Analysis: Uses the all-MiniLM-L6-v2 transformer model to convert raw text into high-dimensional embeddings.

Automated Clustering: Implements K-Means clustering to group complaints based on semantic similarity.

Optimal Cluster Selection: Uses the "Elbow Method" (Within-Cluster Sum of Squares) to determine the ideal number of categories.

Predictive Inference: Includes a predict_root_cause function that assigns new, unseen complaints to the most relevant existing cluster with a confidence score.

🛠️ Tech Stack
Language: Python

Libraries: * pandas & numpy (Data manipulation)

sentence-transformers (NLP Embeddings)

scikit-learn (K-Means Clustering & Similarity)

matplotlib (Visualization)

⚙️ Usage
Load Data: Place your customer_complaints.csv in the same directory as the notebook.

Generate Embeddings: The notebook will download the all-MiniLM-L6-v2 model and encode the complaint text.

Run Clustering: Execute the K-Means cells to identify the optimal number of complaint categories.

Test Predictions: Use the predict_root_cause() function to analyze new complaints
