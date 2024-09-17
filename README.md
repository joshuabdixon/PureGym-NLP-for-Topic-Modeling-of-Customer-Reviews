# NLP for Topic Modelling - Gym Customer Reviews

## Project Overview
This project focuses on using NLP techniques to analyHere's a revised version of the content formatted for a repository README:

---

# Using NLP for Customer Feedback Analysis and Topic Modelling in Fitness Centres

## Project Overview
This project applies Natural Language Processing (NLP) techniques to analyse customer reviews for a global fitness operator (anonymised as "Company X"). The aim is to identify key themes contributing to customer dissatisfaction and extract actionable insights to enhance service quality.

## Problem Statement and Objective
Company X has observed an increase in negative feedback across various review platforms. The project’s objective is to identify common concerns such as cleanliness, equipment quality, customer service, and environmental factors (e.g., noise control). By understanding these themes, the company can implement targeted improvements to enhance the customer experience.

## Statistical Techniques and Libraries
- **Topic Modelling:** Using `BERTopic` and `Gensim` for Latent Dirichlet Allocation (LDA).
- **Emotion Analysis:** Utilising BERT-based models for classifying customer sentiments.
- **Large Language Model (LLM):** Falcon-7b-Instruct to derive actionable insights.
- **Libraries:** `nltk`, `regex`, `wordcloud` for text preprocessing; `transformers` for emotion analysis; `matplotlib` for visualisations.

## Data Overview
The dataset comprises two CSV files containing 12 months of customer reviews: one from Google and the other from Trustpilot.

### Google Reviews Dataset
This dataset contains 23,250 entries, each corresponding to a customer review, with features including:
- **Customer Name:** An anonymised string (not utilised).
- **SurveyID:** A unique identifier (excluded from the analysis).
- **Club’s Name:** The gym's name or location.
- **Creation Date:** The date and time the review was created.
- **Comment:** The customer's review text.
- **Overall Score:** The rating given by the customer (1 to 5 stars).

### Trustpilot Reviews Dataset
This dataset consists of 16,673 entries with similar features, including:
- **Review ID:** A unique identifier (excluded from the analysis).
- **Review Created (UTC):** The date and time of review creation.
- **Review Content:** The full customer review.
- **Review Stars:** The rating given by the customer (1 to 5 stars).
- **Location Name:** The name or location of the gym.

### Assumptions
- Reviews with scores below 3 are considered negative.
- Data is anonymised, and personal identifiers are removed.

## Methodology

### Data Cleaning and Preprocessing
- **Text Cleaning:** Applied regular expressions and basic cleaning to standardise text and remove noise.
- **Tokenisation & Lemmatisation:** Utilised `nltk` for tokenisation, stopword removal, and lemmatisation.
- **Visualisation:** Used word clouds to identify frequently mentioned words and themes.

### Approach
1. **Identifying Common Factors:** Analysed variables such as locations and dates to identify overlaps between Google and Trustpilot reviews.
2. **Topic Modelling:** Implemented `BERTopic` and `Gensim` for clustering reviews, focusing on negative feedback to identify key trends.
3. **Emotion Analysis:** Used BERT-based models to classify emotions in reviews, particularly anger, to understand the driving factors behind negative sentiments.
4. **Generating Insights:** Utilised Falcon-7b-Instruct to generate actionable insights for improving customer experiences.

#### Considerations for Further Analysis
- **Temporal and Spatial Characteristics:** Further analysis of how reviews change over time and across locations could provide deeper insights but was excluded due to time constraints.

## Findings
Recurring themes in negative reviews include:
- **Air Conditioning:** Frequent complaints about temperature control.
- **Noise Control:** Issues with loud music in the gym environment.
- **Cleanliness:** Concerns about maintenance in toilets and changing rooms.
- **Equipment Quality:** Complaints about equipment upkeep and availability.
- **Customer Service:** Reports of negative interactions with staff.

### Emotion Analysis
Anger was identified as the dominant emotion in negative reviews, indicating significant customer dissatisfaction.

## Recommendations
1. **Air Conditioning & Noise Control:**
   - Regularly inspect and maintain air conditioning systems.
   - Implement noise control measures, such as reducing music volume.
2. **Addressing Negative Feedback:**
   - Increase cleaning frequency and hire additional staff for maintenance.
   - Conduct regular equipment inspections and train staff in active listening and problem-solving.
3. **Parking & Accessibility:** 
   - Increase parking availability and ensure systems function correctly to prevent fines.
4. **Priority Locations:** 
   - Address issues at key locations with the highest number of negative reviews to maximise impact.

## Conclusion
This project demonstrates the value of NLP techniques in extracting actionable insights from customer reviews. By addressing the identified concerns, Company X can improve member satisfaction and support business growth. 

For a detailed breakdown of the analysis and methodology, please refer to the Jupyter Notebook in this repository.
