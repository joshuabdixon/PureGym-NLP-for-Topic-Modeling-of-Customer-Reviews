# NLP for Topic Modelling - Gym Customer Reviews

## Project Overview
This project applies Natural Language Processing (NLP) techniques to analyse customer reviews for a global fitness company (anonymised as "Company X"). The objective is to identify key themes in customer dissatisfaction and extract actionable insights to improve service quality and customer experience.

## Problem Statement
Company X has been receiving an increasing number of negative reviews on various platforms. This analysis identifies common concerns such as cleanliness, equipment quality, customer service, and environmental factors like noise control. By uncovering these themes, the company can make informed decisions to address issues and enhance customer satisfaction.

## Statistical Techniques and Libraries
- **Topic Modelling:** Utilised `BERTopic` and `Gensim` (LDA).
- **Emotion Analysis:** Implemented using BERT-based models.
- **Large Language Model (LLM):** Employed Falcon-7b-Instruct to derive actionable insights.
- **Libraries:** `nltk`, `regex`, `wordcloud` for text preprocessing; `transformers` for emotion analysis; `matplotlib` for visualisation.

## Data Overview
The dataset comprises two CSV files containing 12 months of customer reviews from Google and Trustpilot.

### Features
- **Google Reviews Dataset:** 23,250 entries with features like gym location, review date, score, and comments.
- **Trustpilot Reviews Dataset:** 16,673 entries, with similar features including review content, date, and gym location.

## Methodology
1. **Data Cleaning:** Removed unnecessary features, standardised text using regular expressions, and filtered non-English reviews.
2. **Preprocessing:** Tokenised, removed stopwords, and lemmatised reviews using `nltk`.
3. **Topic Modelling:** Applied `BERTopic` and `Gensim` to identify clusters within the reviews, focusing on negative feedback.
4. **Emotion Analysis:** Utilised BERT-based models to classify emotions, particularly ‘anger,’ to understand customer sentiments.
5. **Actionable Insights:** Used Falcon-7b-Instruct to generate recommendations based on identified topics.

### Key Insights
- Frequent concerns include air conditioning issues, noise control, cleanliness, equipment quality, and customer service.
- Anger emerged as the dominant emotion in negative reviews, highlighting strong customer dissatisfaction.

### Recommendations
1. **Air Conditioning & Noise Control:** Regular maintenance of air conditioning and noise reduction strategies.
2. **Cleanliness:** Increase cleaning frequency and employ additional staff for maintenance.
3. **Equipment Quality:** Regularly inspect equipment and provide training for staff to ensure high-quality service.
4. **Parking & Accessibility:** Improve parking facilities and address issues at key locations with high negative feedback.

## Files in This Repository
- **Topic Modelling - Gym Customer Reviews.ipynb:** The Jupyter Notebook containing the complete analysis, including data processing, topic modelling, and visualisation.
- **LICENSE:** The license file for the project.

## Usage
Open the `Topic Modelling - Gym Customer Reviews.ipynb` notebook to review the full analysis and findings. The notebook contains step-by-step explanations, visualisations, and code implementation.

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.
