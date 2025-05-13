**ChatGPT Review Sentiment Analysis**
This project performs sentiment analysis and user complaint categorization on reviews of ChatGPT. 
Using NLP techniques, machine learning models, and data visualization, the project derives meaningful insights and identifies trends in user reviews.


**Overview**
The project analyzes a dataset containing user reviews for ChatGPT. 
It includes sentiment classification (Positive, Neutral, Negative), visualization of sentiment trends over time, extraction of common phrases, and identification of user complaints.

**Workflow**

**Data Preprocessing:**
Removed duplicates and outliers (reviews > 500 words).
Ensured text consistency by treating reviews as strings.
Sentiment Classification:

**Used TextBlob to assign sentiment labels:**
Positive (Polarity > 0)
Neutral (Polarity = 0)
Negative (Polarity < 0)

Converted labels to numerical values for model training:
Positive = 1, Neutral = 0, Negative = -1

Split data into training and test sets (70-30 split).

Trained MultinomialNB for sentiment classification.

**Visualization:**
Sentiment Distribution: Plotted overall sentiment count.
Word Clouds: Generated word clouds for Positive and Negative reviews.
Top Phrases: Extracted and visualized common bigrams/trigrams.
Sentiment Trends: Visualized sentiment variation over time.
User Complaint Identification:

Defined problem categories with associated keywords.
Matched keywords with negative phrases to count occurrences.
Net Promoter Score:

**Calculated NPS based on ratings:**

Promoters (Rating = 5), Passives (Rating = 4), Detractors (others).
Formula: NPS = %Promoters - %Detractors



In this project, we analyze ChatGPT app reviews to understand user sentiment using a combination of TextBlob, TF-IDF, and Naive Bayes. First, we apply TextBlob to each review to obtain a basic sentiment score, giving us a sense of the review’s polarity (positive/negative) and subjectivity. While TextBlob provides a quick, lexicon-based sentiment estimate, we further enhance our analysis using TF-IDF to convert review text into numerical vectors that reflect the importance of each word relative to the entire corpus. These vectors are then fed into a Naive Bayes classifier, which uses probability theory to classify reviews into positive, negative, or neutral categories. By combining both rule-based (TextBlob) and machine learning (TF-IDF + Naive Bayes) approaches, we ensure both interpretability and predictive accuracy in our sentiment analysis pipeline. This hybrid method helps us extract meaningful insights from thousands of user reviews, ultimately supporting better understanding of user feedback and app improvement.

Let me know if you want this paragraph translated into a slide, research abstract, or report section!










