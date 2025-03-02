# AI Discussions Analysis

This repository contains scripts for **scraping, processing, and analyzing** AI-related discussions on Reddit. The pipeline includes **data collection, sentiment analysis, and topic modeling** to gain insights into public attitudes toward AI.

## Repository Structure

### 1. Reddit Data Scraping (`reddit_scraper.ipynb`)
- **Purpose**: Collects posts and comments from AI-related subreddits (`singularity`, `aiwars`).
- **Libraries Used**: `praw`, `pandas`.
- **Key Features**:
  - Fetches posts with AI-related keywords (`AI`, `Machine Learning`, `LLM`, etc.).
  - Extracts metadata: title, content, author, creation date, and URL.
  - Collects comments from posts, handling nested comment structures.
  - Saves data as `combined_posts.csv` and `combined_comments.csv`.

### 2. Sentiment Analysis (`sentiment_analysis.ipynb`)
- **Purpose**: Analyzes the sentiment of posts and comments using `VADER`.
- **Libraries Used**: `vaderSentiment`, `pandas`, `matplotlib`.
- **Key Features**:
  - Computes sentiment scores (`compound`, `positive`, `negative`, `neutral`).
  - Generates sentiment distributions for titles, content, and comments.
  - Saves results as `merged_post.csv` and `merged_comments.csv`.

### 3. Topic Modeling (`topic_modeling.ipynb`)
- **Purpose**: Identifies discussion themes using `Latent Dirichlet Allocation (LDA)`.
- **Libraries Used**: `sklearn`, `gensim`, `matplotlib`, `seaborn`.
- **Key Features**:
  - Preprocesses text (removing stop words, tokenization).
  - Uses **LDA** to identify key topics in AI discussions.
  - Displays top words per topic and sentiment trends across topics.
  - Generates **visualizations**: sentiment distributions and topic density plots.

## Installation & Usage

### Requirements
Ensure you have the required libraries installed:
```bash
pip install praw vaderSentiment pandas scikit-learn gensim matplotlib seaborn
```

### Running the Notebooks
Run the Jupyter notebooks in order:
1. `reddit_scraper.ipynb` → **Scrape Reddit data**
2. `sentiment_analysis.ipynb` → **Analyze sentiment**
3. `topic_modeling.ipynb` → **Discover discussion topics**

## Results & Insights
- Identifies sentiment patterns in AI-related Reddit discussions.
- Highlights **hot topics** and **emerging trends** in AI communities.
- Visualizes sentiment and topic relationships.

## License
This project is licensed under the **MIT License**.

