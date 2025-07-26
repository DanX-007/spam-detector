![image](https://pomf2.lain.la/f/ietrnm3p.jpg)

# How to Use
# load model amd vectorizer
loaded_model = load('spam_classifier_model.joblib')
loaded_vectorizer = load('tfidf_vectorizer.joblib')

# predict new data
new_message = ["Congrats! You won a free ticket"]
X_new = loaded_vectorizer.transform(new_message)
prediction = loaded_model.predict(X_new)

print("Predict:", "spam" if prediction[0] == 1 else "ham")

I'm really lazy to make docs
