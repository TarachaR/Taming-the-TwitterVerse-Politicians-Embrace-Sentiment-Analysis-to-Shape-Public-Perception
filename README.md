# Taming-the-TwitterVerse: Politicians-Embrace-Sentiment-Analysis-to-Shape-Public-Perception
Enhancing Political Brand Reputation Through Twitter Sentiment Analysis

---

>  **Project Authors:** Richard Taracha || Juliet Thuku || Eva Kiio

> **Flatiron School Data Science Program**

>  **Date:** 14/12/2023
> 
![Taming the TwitterVerse](https://github.com/TarachaR/Taming-the-TwitterVerse-Politicians-Embrace-Sentiment-Analysis-to-Shape-Public-Perception/assets/67068918/18cd6417-dd21-450c-9814-fb7b02b2943c)

<p align="right"><i><small>Image by: Richard Taracha</small></i></p>

---
</br>

> ###  Table of Contents
1. [Executive Summary](#background-information) 
2. [Problem Statement](#understanding-the-context)
3. [Proposed Solution](#understanding-the-context)
4. [Data Pertinence and Attribution](#understanding-the-context)
5. [Formulating the Benchmark of Success](#understanding-the-context)
6. [Project Structure & Deliverables](#project-deliverable)
7. [Recording the Experimental Design](#recording-the-experimental-design)
8. [Results](#project-deliverable)


</br>

---

</br>

> ## 1. Executive Summary

***In the dynamic world of politics, public perception plays a crucial role in shaping the success or failure of a political figure. Leveraging the power of social media, particularly Twitter, has become an indispensable tool for political leaders to connect with their constituents, gauge public sentiment, and build a strong brand identity. However, effectively managing and understanding the vast amount of data generated on Twitter can be a daunting task. This is where Twitter sentiment analysis using NLP (Natural Language Processing) emerges as a powerful solution.***

</br>

---
> ## 2. Problem Statement

**Our client, a prominent political figure, seeks to enhance their brand reputation and strengthen their connection with their followers on Twitter. They recognize the importance of understanding public sentiment and identifying emerging trends in online conversations. However, manually analyzing the sheer volume of tweets directed at their account is a time-consuming and resource-intensive endeavor.**

</br>

---
> ## 3. Proposed Solution

**We propose implementing a Twitter sentiment analysis NLP project to automatically extract and analyze sentiment from tweets directed from the client's Twitter account. This solution will provide valuable insights into the public's perception of the client's policies, actions, and overall brand image.**

</br>

---
> ## 4. Data Pertinence and Attribution

**Data Source:**

- Twitter account: Dr. Miguna Miguna (@MigunaMiguna)
- Date range: January 1, 2019 - April 28, 2022
- Number of tweets: 43,479
- Attribution: The data used in this project was scraped from Twitter using Twint, an unofficial Twitter scraper. The data is publicly available on Twitter and is not owned by the author of this project.
- Data Dictionary:

  | Field | Description |
    |-|-|
    | id | Unique identifier for the tweet |
    | conversation_id | Unique identifier for the conversation thread |
    | created_at | Date and time the tweet was created |
    | time | Time zone of the tweet |
    | user_id | Unique identifier for the user who posted the tweet |
    | username | Twitter handle of the user who posted the tweet |
    | name | Name of the user who posted the tweet |
    | place | Location of the user who posted the tweet (if available) |
    | tweet | Content of the tweet |
    | language | Language of the tweet |  
    | mentions | Twitter handles mentioned in the tweet |
    | urls | URLs mentioned in the tweet |
    | photos | Photos attached to the tweet |
    | replies_count | Number of replies to the tweet |
    | retweets_count | Number of retweets of the tweet |
    | likes_count | Number of likes on the tweet |
    | hashtags | Hashtags used in the tweet |
    | cashtags | Cashtags used in the tweet |
    | link | URL of the tweet |
    | retweet | Whether the tweet is a retweet |
    | quote_url | URL of the quoted tweet (if applicable) |
    | video | Whether the tweet includes a video |
    | thumbnail | Thumbnail image for the video (if applicable) |
    | near | Location near which the tweet was posted (if available) |
    | geo | Geolocation coordinates of the tweet (if available) |
    | source | Application used to post the tweet |  
    | user_rt_id | Unique identifier of the retweeted tweet (if applicable) |
    | user_rt | Whether the user retweeted the tweet |
    | retweet_id | Unique identifier of the retweeted tweet (if applicable) |  
    | reply_to | Unique identifier of the tweet being replied to (if applicable) |
    | retweet_date | Date and time the tweet was retweeted (if applicable) |
    | translate | Translated text of the tweet (if applicable) |
    | trans_src | Source language of the translation (if applicable) |  
    | trans_dest | Destination language of the translation (if applicable) |

</br>

---
> ## 5. Formulating the Benchmark of Success

The core benchmarks for success in this NLP Twitter analysis project will be: 

a) Building a classifier accuracy model with at least 80% precision in detecting tweet sentiment (positive, negative, neutral)

b) Providing actionable insights by identifying major influencers, topics, and events impacting changes in sentiment

c) Creating easy-to-understand data visualisations and reports to clearly communicate insights to our client. 

By developing a high-performance classification model and emphasizing practical, strategic business insights, our solution will enable our client to efficiently gauge public perception, track brand reputation, and guide future decisions - achieving their core goal of understanding and connecting with their followers at scale.

</br>

---
> ## 6. Project Structure & Deliverables


</br>

---
> ## 7. Recording the Experimental Design
Adapting the methodology for a Twitter sentiment analysis project involves focusing on the specific aspects related to text data and sentiment classification. Here's a revised methodology for your Twitter sentiment analysis project:

1. **Data Collection and Preprocessing:**
    Gather tweets using relevant usrenames or keywords.
    Preprocess the text data by removing mentions, hashtags, and URLs, and handle special characters.
    Explore the dataset to understand its structure, size, and language-specific nuances.
    Clean the data by addressing issues like spelling errors and removing irrelevant information.

2. **Exploratory Data Analysis (EDA):**
    Perform EDA to understand the distribution of sentiment classes in the dataset.
    Analyze word frequencies, common phrases, and trends in positive, negative, and neutral tweets.
    Identify any patterns or correlations between tweet features and sentiment labels.

3. **Data Visualization:**
    Utilize word clouds, bar charts, and pie charts to visually represent the distribution of sentiments.
    Create visualizations that showcase the most frequent words associated with each sentiment class.

4. **Text Representation:**
    Convert the text data into a suitable format for machine learning models, using TF-IDF.
    Explore different text representation techniques and choose the one that best captures the nuances of sentiment in tweets.

5. **Machine Learning Modeling:**
    Build and train various sentiment analysis models, such as Complement Naive Bayes, Random Forests, and Logistic Regression.
    Evaluate model performance using metrics like accuracy, precision, recall, and F1 score. Here out metric of choice was the Average Macro-Recall Score.
    Address the challenge of imbalanced classes by employing techniques like Random Oversampling.
    Consider the interpretability of the models, especially if explaining the results is important.

6. **Hyperparameter Tuning and Model Selection:**
    Fine-tune the hyperparameters of the chosen model to optimize performance.
    Select the model that demonstrates the best balance between precision and recall for sentiment classification.

7. **Deployment:**
    Deploy the chosen model as a Streamlit Web application to perform sentiment analysis on incoming tweets.

8. **Results Interpretation and Reporting:**
    Interpret the model predictions and analyze any misclassifications.
    Provide insights into the most influential features or words contributing to each sentiment class.
    Summarize the overall findings in a clear and concise manner suitable for sharing on Twitter or other platforms.




</br>

---
> ## 8. Results
