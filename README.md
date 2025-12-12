# 📘 YouTube Comment Emotion Analyzer

This project is a small Machine Learning model that can predict the **emotion** behind a YouTube comment.  
I created this mainly for learning purposes and to practice basic text processing and classification.

The model can identify these emotions:

- **Joy**
- **Anger**
- **Sadness**
- **Fear**
- **Love**
- **Neutral**

I used a simple dataset of comments (with emojis included) and trained a Naive Bayes classifier on top of it.

## 📂 Project Contents

```
youtube-emotion-analyzer/
│
├── data/comments.csv        → Small dataset of YouTube-style comments
├── emotion_analyzer.ipynb   → Main Jupyter notebook with code
├── requirements.txt         → Python packages used
└── README.md                → Project documentation
```

## 🚀 How I Ran the Project

1. Installed the required libraries:
   ```
   pip install -r requirements.txt
   ```
2. Opened the notebook:
   ```
   jupyter notebook
   ```
3. Ran all cells to train the model and test emotion predictions.

## 🧠 What the Notebook Does

- Cleans the text (removes symbols, converts emojis into words, etc.)
- Converts text into numerical features using **CountVectorizer**
- Splits the data into training and testing sets
- Trains a Naive Bayes classifier
- Prints accuracy and confusion matrix
- Lets you test your own comment like:
  ```python
  predict_emotion("This video made me laugh 😂")
  ```

## ✔️ Example Output

For a comment like:

```
"This video is so funny 😂😂"
```

The model returns:

```
joy
```

## 🎯 Why I Made This

I wanted a beginner-friendly project that:
- uses Python + ML  
- includes NLP and emojis  
- looks good on GitHub  
- is simple but still useful  

This project helped me understand text preprocessing and basic classification models.

## 📌 Future Improvements (If I get time)

- Use a bigger dataset  
- Try deep learning models like LSTM  
- Deploy as a small web app  
