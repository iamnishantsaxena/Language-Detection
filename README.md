## Language Detection with Text Preprocessing and Multinomial Naive Bayes

This Python script implements a language detection system using text pre-processing and the Multinomial Naive Bayes classification algorithm. 

**Skills Used:**

* **Data Analysis Libraries:** pandas
* **Natural Language Processing (NLP):** Text pre-processing techniques (regular expressions)
* **Machine Learning:**
    * Feature Extraction: CountVectorizer (Bag-of-Words)
    * Model Training: Multinomial Naive Bayes
    * Model Evaluation: Accuracy score, confusion matrix, classification report
* Model Persistence: pickle (for saving and loading the trained model)

**Functionality:**

1. **Data Loading:** Loads the language data from a CSV file ("Language Detection.csv").
2. **Model Loading (if exists):**
   * Attempts to load a pre-trained model from a specified file path (`model_path`).
   * If the model is not found, it proceeds to training.
3. **Text Preprocessing:**
   * Defines a function `preprocess_text` to:
      * Remove special characters and punctuation.
      * Convert text to lowercase.
4. **Feature Extraction:**
   * Transforms text data into numerical features using CountVectorizer (Bag-of-Words).
5. **Model Training (if necessary):**
   * Splits data into training and testing sets.
   * Trains a Multinomial Naive Bayes model on the training data.
   * Saves the trained model for future use.
6. **Prediction:**
   * Predicts the language labels for unseen text data (test set).
7. **Evaluation:**
   * Calculates accuracy score, confusion matrix, and classification report to assess model performance.
8. **Custom Sentence Prediction (Optional):**
   * Provides a function `predict_custom` to predict language labels for a list of user-defined sentences.

**Instructions:**

1. Ensure you have the required libraries installed.
2. Replace `"Language Detection.csv"` with the actual path to your data file.
3. Modify the `model_path` variable to specify where the trained model should be saved/loaded.
4. Run the script.

**Additional Information:**

* The code utilizes regular expressions for text pre-processing. You can explore more advanced NLP libraries for richer text manipulation capabilities.

* Multinomial Naive Bayes is a simple yet effective algorithm for text classification tasks. Other machine learning algorithms might be explored for potentially improved performance.

