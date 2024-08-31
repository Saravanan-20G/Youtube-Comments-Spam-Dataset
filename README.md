# 🎥 YouTube Comment Analysis Project

## Overview

This project analyzes YouTube video comments to understand comment distribution, user engagement, sentiment, and spam detection effectiveness. It involves Exploratory Data Analysis (EDA), sentiment analysis, and a machine learning model to classify comments as spam or not. A Streamlit application provides an interactive way to visualize the results.

## Dataset

- **Source**: `"YouTube-Spam-Dataset.csv"`
- **Columns**:
  - **`COMMENT_ID`**: Unique identifier for each comment.
  - **`AUTHOR`**: Name of the comment's author.
  - **`DATE`**: Date when the comment was posted.
  - **`CONTENT`**: Text content of the comment.
  - **`CLASS`**: Spam label (1 for spam, 0 for non-spam).
  - **`VIDEO_NAME`**: Video associated with the comment.

## Project Structure

1. **Data Preprocessing**:
   - Handling missing values and data types.
   - Checking for duplicates.
   
2. **Exploratory Data Analysis (EDA)**:
   - Class distribution, most commented videos, top commenters.
   - Comment length distribution and word cloud visualization.
   - Temporal analysis of comments over time.
   
3. **Sentiment Analysis**:
   - Sentiment polarity calculated using TextBlob.
   - Visualization of sentiment polarity distribution.

4. **Model Building**:
   - Vectorization of comments using TfidfVectorizer.
   - Random Forest Classifier for spam detection.
   - Evaluation using confusion matrix, ROC curve, and classification report.

5. **Visualization**:
   - Streamlit app for interactive exploration.

## Installation & Requirements

Install the required libraries:

```bash
pip install pandas numpy seaborn matplotlib plotly scikit-learn wordcloud textblob streamlit



## Usage

Run the EDA and Model Building

Prepare the Data: Load and preprocess the dataset by running the preprocessing and EDA scripts.

Train the Model: Execute the model training script to train and evaluate the spam detection model.

## Results

Model Accuracy: High accuracy in spam vs. non-spam classification.

Insights:

Distribution of Comments: Shows engagement patterns across videos and authors.

Sentiment Analysis: Provides insights into audience reactions.

Spam Detection: Effective for moderating comments.
