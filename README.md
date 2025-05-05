# Real-Time-Cyber-Bullying-Analysis

This project analyzes tweets in **real-time** using a fine-tuned `DistilBERT` transformer model to detect and classify cyberbullying. Built using the Hugging Face Transformers library and `tweepy`, this solution attempts to flag potentially harmful tweets as they are posted—serving as a **safety net** for social platforms like X (formerly Twitter).

## 📌 Project Overview

The primary goal of this project is to detect **cyberbullying across six categories**:

- Age-based bullying  
- Ethnicity-based bullying  
- Gender-based bullying  
- Religion-based bullying  
- Other types of bullying  
- Not cyberbullying

The dataset used for training is sourced from Kaggle:  
👉 [Cyberbullying Classification Dataset](https://www.kaggle.com/datasets/andrewmvd/cyberbullying-classification)

## ⚙️ Technologies Used

- `DistilBERT` (Hugging Face Transformers)
- `PyTorch`
- `NLTK`
- `Tweepy` for Twitter API
- `Torch` and `tokenizers` for preprocessing

## 🧠 Model Training

- The model was trained on a cleaned and preprocessed dataset of ~47,000 tweets.
- Data was balanced across classes (~8000 tweets each).
- Input sequence length: 64 tokens.
- Achieved best training accuracy: **82.69%** on epoch 3.

## 📡 Real-Time Tweet Classification

Using `tweepy`, this system streams tweets based on hashtags or keywords and classifies them **on-the-fly** using the trained model. Each tweet is labeled into one of the six categories defined above.

## 🎥 Demo Video

➡️ [Watch the video here](https://youtu.be/kxBgn8cdJEQ) 

## 🚧 Challenges Faced

- Low separability between `other_cyberbullying` and `not_cyberbullying`
- API rate limitations from Twitter/X
- Sarcasm and slang affect classification accuracy
- Deciding ethical boundaries for censoring content

## ✅ Conclusion

This project highlights the importance—and the difficulty—of identifying harmful speech online. It is not meant to censor but to **caution**, offering a chance to rethink before posting something potentially hurtful. As Elon Musk’s vision reshapes platforms like X, AI tools like this can help maintain respectful discourse.

## 📚 References

1. Tweepy Documentation – [https://docs.tweepy.org/](https://docs.tweepy.org/)
2. Hugging Face Transformers Documentation – [https://huggingface.co/docs/transformers](https://huggingface.co/docs/transformers)
3. Kaggle Dataset: Cyberbullying Classification – [https://www.kaggle.com/datasets/andrewmvd/cyberbullying-classification](https://www.kaggle.com/datasets/andrewmvd/cyberbullying-classification)


**No to Online Hate!**

---

**Developed by:** Pratham V K  
**Course:** MFG 598 – Real-Time Tweet Analysis  
