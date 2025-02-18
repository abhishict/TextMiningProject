# **Electric Vehicles: Public Perception Analysis**  

## **Project Overview**  
This project analyzes **public opinion and discourse on Electric Vehicles (EVs)** by collecting and processing text data from **news articles, Reddit discussions, and web sources**. The goal is to understand **key concerns, benefits, and trends** in EV adoption using **Natural Language Processing (NLP) and machine learning techniques**.  

---

## **Dataset & Sources**  
Data was collected from:
- **NewsAPI** (EV-related news articles from sources like BBC, The Guardian, and TechCrunch)
- **The Guardian Web Scraping** (Articles from the “EV Mythbusters” series)
- **Reddit API** (Discussions from subreddits like r/electricvehicles, r/cars, r/sustainability)

Each entry in the dataset contains:
- **Label:** Classification of the text into categories such as *Environmental Benefit, Economic Challenge, etc.*
- **Cleaned_Description:** Processed textual content after text cleaning.

---

## **Data Processing Steps**  
1. **Text Cleaning**: Removed punctuation, stopwords, URLs, and applied lemmatization.  
2. **Feature Extraction**: Used **CountVectorizer (CV)** and **TF-IDF** to convert text into numerical features.  
3. **Categorization**: Applied **zero-shot classification** and **semantic similarity** to label text into:  
   - *Environmental Benefit, Environmental Concern, Economic Advantage, Economic Challenge.*  

---

## **Exploratory Data Analysis (EDA)**  
Several visualizations were created to explore trends, including:
- **Word Clouds**: Displaying the most common words in **Pro-EV and Against-EV** discussions.
- **Label Distribution**: Bar chart showing **how different opinions are represented**.
- **Bigram Analysis**: Finding the most common two-word phrases in **Environmental Concern vs. Benefit** discussions.
- **Article Length Distribution**: Understanding the variation in text length across sources.

---

## **How to Run the Project**
1. **Install Dependencies**:
   ```bash
   pip install pandas numpy matplotlib seaborn nltk sklearn transformers beautifulsoup4 requests praw wordcloud
   ```

---
