# PCA-MDS-LDA-Sentiment
University assignment referring to the Text Analytics course.

# Text Analytics for Marketing: Group Assignment 1 - Understanding Text Data

** Ioannis Nikolaidis**  
_Date_: March 31, 2023

## 1. Introduction

In today’s digital age, online reviews have become an essential part of consumers’ decision-making processes. Analyzing this data has become crucial for businesses aiming to grasp customer opinions and enhance their offerings. This project employs techniques such as principal component analysis (PCA), multi-dimensional scaling (MDS), sentiment analysis, and latent Dirichlet allocation (LDA) to interpret the sentiments conveyed by customers and to pinpoint key topics in the reviews.

## 2. Data Description

Textual data from Delta airline reviews were the foundation for this analysis. Key features of this dataset include:

- A star rating scale ranging from 1 to 10, with 10 being the peak rating.
- Each star rating is paired with a textual review and is associated with a unique customer ID.
- Two dataset versions: 
  - One retained its original form, inclusive of punctuation and without stemming, for sentiment analysis.
  - A fully sanitized version (removal of punctuation, stemming, tokenization, and stripping of stop words) for the bulk of the analysis.

## 3. Analysis

### 3.1 Principal component analysis (PCA)

PCA aims to pinpoint the components with utmost predictive accuracy that effectively capture the essence of reviews in a high-dimensional space. Major findings include:

- The first five principal components (PCs) seem to tackle themes like:
  - PC1: Time and logistical aspects of travel.
  - PC2: Passenger amenities and comfort.
  - PC3: Luggage-related topics.
  - PC4: Travel disruptions.
  - PC5: Interactions with airline staff.
  
- Rotation techniques improved interpretability. See Figure 1 for details.

> **Figure 1**: Biplots of the first 4 dimensions.

### 3.2 Multi-Dimensional Scaling (MDS)

MDS visually depicts word similarities on a 2D or 3D plane. Three separate MDS tests were conducted, each with varying contexts. Key observations:

- The plot with the context set to "document" revealed the most distinct clusters, as depicted in Figure 3.
  
> **Figure 3**: Word Map.

### 3.3 Comparison of PCA and MDS

While both PCA and MDS are adept at summarizing word vector data's intrinsic structure, their methodologies and outputs differ significantly. For our dataset, PCA provided a clearer visualization over MDS.

### 3.4 Sentence Based Sentiment Analysis using the Polarity Algorithm

Sentiment analysis, leveraging the Jockers & Rinker dictionary, revealed:

- A noticeable volume of negative reviews over positive ones.
- A mismatch between sentiment scores and star ratings, hinting at the unreliability of the latter. See Figure 5 for detailed insights.

> **Figure 5**: Sentiment score by star rating.

### 3.5 Latent Dirichlet Allocation (LDA)

LDA identified the optimal number of topics as 5. Each topic was then labeled based on the predominant terms, as seen in Figure 8.

> **Figure 8**: Top 10 terms of the first 5 topics.

## 4. Conclusions

Analyzing Delta airline reviews using PCA, MDS, Sentiment Analysis, and LDA furnished vital insights into customer sentiments and spotlighted pivotal review topics. Such techniques are instrumental for businesses striving to fathom customer feedback and refine their offerings.


