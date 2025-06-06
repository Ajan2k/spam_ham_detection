# Spam Detection using Machine Learning

This project implements a spam/ham email classifier using natural language processing (NLP) and machine learning techniques. The workflow includes data preprocessing, feature extraction with TF-IDF, class balancing with SMOTE, model training, and evaluation.

## Project Structure

```
.
├── data/
│   └── mail_data.csv
├── spam_det.ipynb
├── requirements.txt
└── README.md
```

## Features

- **Text preprocessing**: Tokenization, lemmatization, and stopword removal using spaCy.
- **Feature extraction**: TF-IDF vectorization of email text.
- **Class balancing**: SMOTE oversampling to handle class imbalance.
- **Model training**: Random Forest and Logistic Regression classifiers.
- **Evaluation**: Accuracy, confusion matrix, and classification report.
- **Visualization**: Category distribution plots.

## How to Run

1. **Clone the repository**  
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

2. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   python -m spacy download en_core_web_sm
   ```

3. **Place your dataset**  
   - Put your `mail_data.csv` file in the `data/` folder.

4. **Run the notebook**  
   - Open `spam_det.ipynb` in Jupyter Notebook or VS Code and run all cells.

## Dataset

- The dataset should be a CSV file with at least two columns:  
  - `Message`: The email text.
  - `Category`: The label (`spam` or `ham`).

## Results

- The notebook will output model accuracy, confusion matrix, and classification report.
- You can test the model with custom email samples.

## Requirements

- Python 3.7+
- pandas
- scikit-learn
- imbalanced-learn
- spaCy
- matplotlib
- ydata-profiling (optional, for EDA)

## License

This project is for educational purposes.
