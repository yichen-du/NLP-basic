# Reddit Comments Analysis

## 📌 Project Overview
This repository contains data and code for analyzing comments from the subreddit **ChangeMyView (CMV)**. The project involves downloading, processing, and topic modeling using **Natural Language Processing (NLP) techniques**.

### **Goals**
- 📥 Download and preprocess Reddit comments from **ChangeMyView** subreddit.
- 📝 Perform **tokenization, stopword removal, and lemmatization** using **spaCy**.
- 🧠 Apply **Latent Dirichlet Allocation (LDA)** for topic modeling.
- 🔍 Identify key topics and find the most relevant comments per topic.
- 💾 Save the processed data for further analysis.

---

## 📂 Data Source
The dataset is sourced from a publicly available file on GitHub:
```
https://raw.githubusercontent.com/dhh2024/disc/main/data/work/samples/cmw_comments_sample_1.tsv
```
It contains Reddit comments along with metadata such as **subreddit, author, timestamp, score, and comment body**.

---

## ⚙️ Installation & Dependencies
To run the code, install the required Python libraries:
```bash
pip install pandas requests spacy gensim nltk
python -m spacy download en_core_web_sm
```

---

## 🚀 Usage
1️⃣ **Download Data**: Fetches Reddit comments from GitHub and loads them into a Pandas DataFrame.
2️⃣ **Preprocess Text**:
   - 🔠 Convert text to lowercase.
   - 🚫 Remove stopwords and punctuation.
   - 🔄 Apply lemmatization using **spaCy**.
3️⃣ **Topic Modeling**:
   - 🔗 Convert processed text into tokens.
   - 📚 Create a dictionary and corpus using **Gensim**.
   - 🏷 Train an **LDA model** to identify topics.
   - 📊 Extract the top **5** topics and their most relevant comments.

---

## 📌 Example Output
After processing, the script generates:
- ✅ **Top topics with key terms.**
- ✅ **List of most relevant comments for each topic.**
- ✅ **A CSV file (`top_themed_comments.csv`)** storing the top comments per topic.

---

## 📁 Files in the Repository
📌 `main.py` - Main script for fetching, processing, and modeling the data.
📌 `top_themed_comments.csv` - Output file with top comments for each identified topic.
📌 `requirements.txt` - List of dependencies (optional).

---

## 🚀 Future Improvements
- 🔥 Expand topic modeling to include **more topics**.
- 📊 Implement **sentiment analysis** on comments.
- 🎨 Create **interactive visualizations** of topic distributions.

---

## 👤 Author
Yichen Du
## 📜 License
This project is licensed under the **MIT License**.

