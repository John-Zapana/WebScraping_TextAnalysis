# Learning web scraping and text analysis

## Part 1: Web Scraping
Research and Comparison of Web Scraping Libraries

### 1. Scrapy:
- Pros:
    - Efficient for large-scale scraping due to its asynchronous nature.
    - Comprehensive framework with built-in support for handling requests, following links, and storing data.
    - Extensive documentation and community support.
- Cons:
    - Steeper learning curve compared to other libraries.
    - Overhead for small projects due to its comprehensive framework.

### 2. BeautifulSoup:
- Pros:
    - Easy to learn and use, especially for beginners.
    - Flexible and can be combined with the requests library for fetching pages.
    - Suitable for small to medium-sized projects.
- Cons:
    - Slower than Scrapy for large-scale projects due to its synchronous nature.
    - Requires additional libraries for handling requests and browser automation.

### Recommendation
For this project, **BeautifulSoup** combined with Requests is recommended due to its ease of use within a Jupyter Notebook environment. While it may not be as fast as Scrapy for very large-scale scraping, it is sufficient for collecting 100 pages, especially if the pages are static.

## Part 2: Text analysis
We'll use two algorithms to analyze the data collected in Part 1. We'll perform **sentiment analysis** and **topic modeling** to generate summaries and importance scores for each article.

### 1. Sentiment Analysis
- We'll use TextBlob to determine the sentiment of each article's title. This will help assign a positive or negative direction to the importance score.

### 2. Topic Modeling
- We'll use gensim for LDA (Latent Dirichlet Allocation) to identify topics within the articles.
- This can help in summarizing the content and determining its relevance to our chosen topic.

## Summary

### Part 1: Web Scraping
- **Objective:**  
The goal was to collect at least 100 articles or pages on a specific topic from public sites.
- **Methodology:**  
We used `BeautifulSoup` and `Requests` to scrape titles and URLs from multiple subreddits related to machine learning and AI.
- **Outcome:**  
Successfully collected 129 titles, focusing on topics like machine learning, AI, and data science.

### Part 2: Text Analysis
- **Objective:**  
Analyze the collected titles to extract sentiment and thematic insights.
- **Sentiment Analysis**
    - **Average Importance Score:** Approximately 1.09, indicating a slight positive sentiment.  
    - **Distribution:** Most titles had neutral sentiment, with scores clustering around zero.
- **Topic Modeling**
    - **Common Topics:** "Learning," "machine," "AI," "ML," and "engineer" were identified as key themes.  
    - **Prevalence:** These topics were consistently present across the dataset, highlighting a focus on technology and innovation.

## Conclusion
- The Assignment effectively demonstrated the use of web scraping and text analysis to gather and interpret data from online sources. The neutral sentiment trend and the emphasis on machine learning and AI topics reflect the dataset's focus on technology. These insights can inform content strategy, research focus, or further exploration in related fields.
- The approach showcased the power of combining data collection with analytical techniques to derive meaningful insights from textual data.
