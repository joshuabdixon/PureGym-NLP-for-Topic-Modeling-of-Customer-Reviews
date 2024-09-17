# Topic Modelling - Gym Customer Reviews

## Project Overview
This project focuses on using NLP techniques to analyse customer reviews for a gym company, identifying key themes and patterns. The goal is to extract insights from the reviews, allowing the company to make data-driven decisions to enhance service quality and customer satisfaction. The analysis is based on real data, and the gym has been anonymised for the purpose of this portfolio.

## Contents
1. **Problem Statement and Objective**: The gym company is experiencing varied customer feedback through online reviews. This project employs topic modelling and sentiment analysis to identify the main themes in these reviews, especially focusing on negative feedback, to improve customer experience and operational efficiency.
   
2. **Statistical Techniques and Libraries**: 
    - **Techniques**:
        - **Topic Modelling**: Using BERTopic, Falcon-7b-Instruct, and Latent Dirichlet Allocation (LDA) to uncover main themes in reviews.
        - **Emotion Analysis**: Applying a BERT-based model to detect emotions, highlighting areas of customer dissatisfaction.
    - **Python Libraries**:
        - `numpy`, `pandas` for data manipulation.
        - `matplotlib.pyplot` for data visualisation.
        - `nltk` for text processing.
        - `bertopic`, `gensim`, and `transformers` for topic modelling and emotion analysis.
   
3. **Key Variables and Assumptions**:
    - **Variables**:
        - **Review Content**: The text of customer reviews.
        - **Review Score**: Ratings given by customers, ranging from 1 to 5 stars.
        - **Location**: The location of the gym associated with the review.
    - **Assumptions**:
        - Only English-language reviews were considered.
        - Reviews scoring below 3 stars are classified as negative.

4. **Data Summary**:
    - The dataset includes 12 months of customer reviews from online platforms.
    - Reviews detail customer experiences, rating scores, and gym locations.

5. **Topic Modelling**:
    - The analysis used three different approaches: BERTopic, Falcon-7b-Instruct, and LDA, each providing unique insights into the customer feedback.
    - **Findings**:
        - Common themes across all reviews included air conditioning, noise control, cleanliness, equipment quality, and customer service.
        - Negative reviews predominantly mentioned issues related to gym cleanliness, staff interactions, and parking availability.

6. **Recommendations**:
    - **Air Conditioning and Noise Control**:
        - Schedule regular inspections and maintenance of air conditioning systems.
        - Reduce music volume in gyms and soundproof exercise rooms.
    - **Addressing Negative Reviews**:
        - Implement stricter cleaning schedules and hire additional staff to maintain cleanliness in facilities.
        - Conduct regular equipment inspections and modernise outdated equipment.
        - Train staff in customer service skills and establish standardised service policies.
    - **Parking & Accessibility in High-Complaint Locations**:
        - Improve parking systems, enhance signage, and ensure clear guidelines to avoid fines.
    - **Priority Locations**:
        - Focus efforts on addressing issues at key locations identified in the analysis, such as "Location A" and "Location B".

7. **Conclusion**: Implementing the recommendations based on topic modelling and sentiment analysis will help improve customer satisfaction and attract new members.

## Files Included in This Repository
- **Notebook**: A detailed Jupyter Notebook ("Topic Modelling - Gym Customer Reviews.ipynb") containing the full implementation of the topic modelling and sentiment analysis.
- **MIT LICENSE**: The license for this project.

## Usage
Feel free to explore the code and analysis to gain insights into the approach used for customer feedback analysis. If you have any questions or would like to discuss job opportunities, please contact me.
