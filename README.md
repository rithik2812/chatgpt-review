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
