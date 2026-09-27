# 😃 Tweet Sentiment & Emoji Analyzer

## 📌 Project Overview
This project performs sentiment analysis on a dataset of tweets containing emojis. Because emojis carry significant emotional weight, the script maps each emoji to its descriptive Unicode name before processing the text. Using TF-IDF vectorization and a Logistic Regression model, the project predicts whether a tweet is positive or negative, achieving an 80% accuracy rate. It also features a real-time interactive widget built with `ipywidgets` that allows users to type sentences and instantly see the predicted sentiment.

## 🗄️ Dataset
* **Source Datasets:** `1k_data_emoji_tweets_senti_posneg.csv` and `15_emoticon_data.csv`.
* **Features:** Contains tweet text, binary sentiment labels (0 = Negative, 1 = Positive), and emoji UTF-8 references.

## 🛠️ Methodology & Tools
* **Data Cleaning:** Dynamically replaces emojis in the text with their exact Unicode string descriptions using a mapped dictionary.
* **Feature Extraction:** Utilizes `TfidfVectorizer` (capped at 10,000 max features) to convert the cleaned text into numerical format.
* **Modeling:** Trains a `LogisticRegression` classifier on an 80/20 train-test split.
* **Interactive UI:** Deploys `ipywidgets` directly inside the notebook to intake real-time user string inputs and output continuous sentiment predictions.

## 📁 Repository Structure
* `text-sentiment-analysis.ipynb`: The complete Python codebase containing the emoji mapping, TF-IDF vectorization, model training, evaluation metrics, and the interactive widget.
* `1k_data_emoji_tweets_senti_posneg.xlsx` / `.csv`: The dataset used for model training and testing.
