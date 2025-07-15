# Language Identifier - UKP

This is a simple language identification project for the UKP Lab internship task, using a dataset from Kaggle. The goal is to predict the language of a given sentence using a machine learning model trained on TF-IDF features.

## 🔍 Dataset

The dataset used in this project was taken from Kaggle:
[Language Identification Dataset](https://www.kaggle.com/datasets/zarajamshaid/language-identification-datasst)

It contains sentences labeled by language in over 20 different languages including English, French, Persian, Hindi, and more.

## 🧠 Model

The model was built using the following steps:
- Text preprocessing
- TF-IDF vectorization
- Model training with Logistic Regression
- Evaluation using classification report

## 📊 Results

The model achieved an accuracy of **96%** on the test set. It performed especially well on languages like Persian, Hindi, and Turkish, but had slightly lower performance on languages like Chinese and Japanese.

## 💬 Test Your Own Sentences

You can use the following code snippet to test a custom sentence:

```python
test_sentence = ["سلام حال شما چطوره؟"]
predicted_language = model.predict(test_sentence)
print("Predicted language:", predicted_language[0])
