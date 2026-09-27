# 😃 Tweet Sentiment & Emoji Analyzer

## 📌 Project Overview
This project performs sentiment analysis on a dataset of tweets containing emojis[cite: 13]. Because emojis carry significant emotional weight, the script maps each emoji to its descriptive Unicode name before processing the text[cite: 13]. Using TF-IDF vectorization and a Logistic Regression model, the project predicts whether a tweet is positive or negative, achieving an 80% accuracy rate[cite: 13]. It also features a real-time interactive widget built with `ipywidgets` that allows users to type sentences and instantly see the predicted sentiment[cite: 13].

## 🗄️ Dataset
* **Source Datasets:** `1k_data_emoji_tweets_senti_posneg.csv` and `15_emoticon_data.csv`[cite: 13].
* **Features:** Contains tweet text, binary sentiment labels (0 = Negative, 1 = Positive), and emoji UTF-8 references[cite: 13].

## 🛠️ Methodology & Tools
* **Data Cleaning:** Dynamically replaces emojis in the text with their exact Unicode string descriptions using a mapped dictionary[cite: 13].
* **Feature Extraction:** Utilizes `TfidfVectorizer` (capped at 10,000 max features) to convert the cleaned text into numerical format[cite: 13].
* **Modeling:** Trains a `LogisticRegression` classifier on an 80/20 train-test split[cite: 13].
* **Interactive UI:** Deploys `ipywidgets` directly inside the notebook to intake real-time user string inputs and output continuous sentiment predictions[cite: 13].

## 📁 Repository Structure
* `text-sentiment-analysis.ipynb`: The complete Python codebase containing the emoji mapping, TF-IDF vectorization, model training, evaluation metrics, and the interactive widget[cite: 13].
* `1k_data_emoji_tweets_senti_posneg.xlsx` / `.csv`: The dataset used for model training and testing[cite: 13].
