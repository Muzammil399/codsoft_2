#  Stop the Junk! — SMS Spam Filter

##  What Is This Project?

This is a simple yet powerful machine learning project designed to automatically sort your text messages into **Ham (Legitimate)** or **Spam**.  

It’s a complete end-to-end pipeline that takes messy text messages and turns them into clean, understandable data for an intelligent, accurate spam filter.

---

##  How It Works

Here’s what happens behind the scenes:

###  1. Text Cleaning  
We start by cleaning up every message using **Natural Language Processing (NLP)**.  
This involves:
- Removing punctuation, numbers, and special characters  
- Getting rid of common filler words (like *the*, *is*, *and*)  
- Reducing words to their root form (for example, *running* → *run*)  

###  2. Feature Extraction with TF-IDF  
Once the text is clean, we convert it into numbers using **TF-IDF (Term Frequency–Inverse Document Frequency)**.  
This technique highlights important words that are strong spam indicators — like *WINNER* or *CLAIM NOW* — while downplaying common words.

###  3. Model Training  
The cleaned and vectorized messages are then fed into a **Logistic Regression** model.  
This algorithm learns the difference between spam and legitimate texts.  
It’s tuned to prioritize **Recall**, meaning it catches as many spam messages as possible without letting them slip through — while still maintaining high accuracy.

---

