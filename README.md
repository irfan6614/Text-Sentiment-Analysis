Task 2: Text Sentiment Analysis
Project Overview:
This project performs **Sentiment Analysis** on the IMDB movie review dataset using **Natural Language Processing (NLP)** and **Machine Learning**. The goal is to classify user reviews as **positive** or **negative** by training a classifier on pre-labeled data.
Dataset Used:
**IMDB Dataset.csv**
Contains two columns:
review`: The text of the movie review.
sentiment`: The label (`positive` or `negative`).
Project Steps:
1. **Data Loading**  
   Read the IMDB dataset into a DataFrame.

2. **Label Encoding**  
   Convert categorical sentiment (`positive`/`negative`) to binary values (`1`/`0`).

3. **Data Splitting**  
   Use an 80/20 train-test split.

4. **Text Vectorization**  
   Transform raw text into numerical features using **TF-IDF Vectorization** (limit 5000 features).

5. **Model Training**  
   Train a **Multinomial Naive Bayes** classifier using the TF-IDF features.

6. **Model Evaluation**  
   Evaluate using `precision`, `recall`, `f1-score`, and `accuracy`
How to Run:
1.	Prerequisites
Make sure you have the following Python libraries installed:
```bash
pip install pandas scikit-learn
2.	Run the Script
Save the code into a Python file, e.g., sentiment_analysis.py, and run:
python sentiment_analysis.py
       Ensure the dataset file is named IMDB Dataset.csv and is in the same directory (or update the      file path in the script).
Sample Output
 
Observations
•  The Naive Bayes classifier performs well with an accuracy of ~88%.
•  TF-IDF is effective for converting reviews into numerical form while ignoring common stopwords.
•  Performance could improve further using deep learning models like LSTM or BERT.

