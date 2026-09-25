# Decoding Smartphone Distraction: Analysing Notification and Usage Patterns

## 1. Problem Statement

Smartphone distraction is often measured using screen time alone. However, screen time does not explain how frequently users check their phones, how many notifications they receive, whether they check their phones without receiving a new notification, or how often smartphone activity interrupts study or work.

This project analyses smartphone usage and notification behaviour to identify different behavioural patterns and provide practical digital-wellbeing recommendations.

## 2. Objectives

- Analyse smartphone usage and notification behaviour.
- Identify relationships between smartphone usage, notifications and interruptions.
- Use K-means clustering to identify smartphone distraction patterns.
- Use Random Forest classification to predict frequent study/work interruptions.
- Provide practical recommendations based on the identified behavioural patterns.

## 3. Data Collection

### Source

Google Forms questionnaire:

**Smartphone Usage & Distraction Behaviour Survey**

Approximately 140 responses were initially collected through the questionnaire. These responses were used as the basis for preparing the final 10,000-record analytical dataset.

### Main Variables

- Daily smartphone usage
- Daily phone checks
- Daily notifications
- Phantom checking
- Work/study notification percentage
- Social/entertainment notification percentage
- Study/work interruption frequency
- Concentration
- Productivity decrease
- Digital-wellness feature usage

## 4. Analytics Methods Used

### Data Preparation
- Data cleaning
- Handling missing values
- Converting categorical/range-based responses into numerical values
- Feature standardization

### Exploratory Data Analysis
- Distribution analysis
- Behavioural pattern analysis
- Spearman correlation analysis

### K-Means Clustering

K-means clustering was used to identify groups of users with similar smartphone usage and notification behaviour.

Different values of K were evaluated using the silhouette score. K = 3 produced the highest silhouette score of 0.1386. However, K = 2 was retained for the final behavioural analysis to obtain two broad and easier-to-interpret distraction segments.

### Random Forest Classification

Random Forest was used to predict users with frequent study/work interruptions.

The model was evaluated using:

- Accuracy: 58.1%
- Precision: 52.13%
- Recall: 47.71%
- F1-score: 49.82%

## 5. Key Results

### K-Means Clustering

The final analysis produced two broad behavioural segments.

**Cluster 0 – Lower Smartphone Distraction**

- Lower screen time
- Fewer notifications
- Lower study/work interruption levels

**Cluster 1 – Higher Smartphone Distraction**

- Higher screen time
- More frequent phone checking
- Higher notification exposure
- Higher study/work interruption levels

The clusters are treated as descriptive behavioural segments rather than fixed personality types.

### Random Forest

The Random Forest model was evaluated on a held-out test set to predict frequent study/work interruptions.

The classification performance is reported using accuracy, precision, recall and F1-score in the project notebook and case study report.

## 6. Business Recommendations

- Use notification batching and priority filtering for users with high notification exposure.
- Encourage screen-time monitoring for high-usage users.
- Use scheduled focus periods and Do Not Disturb during study/work periods.
- Reduce unnecessary notifications to limit repeated phone checking.
- Provide behaviour-based digital-wellbeing recommendations rather than applying the same intervention to every user.

## 7. References

1. Zhou, Y., & Deng, L. (2024). *Breaking free from the “digital rabbit hole”: A configurational analysis of in-class smartphone distraction among university students*. The Internet and Higher Education, 62, 100949.

2. *Electrophysiological effects of smartphone notifications on cognitive control following a brief mindfulness induction*. (2024). Biological Psychology, 185, 108725.

3. Paterna, A., Alcaraz-Ibáñez, M., Aguilar-Parra, J. M., Salavera, C., Demetrovics, Z., & Griffiths, M. D. (2024). *Problematic smartphone use and academic achievement: A systematic review and meta-analysis*. Journal of Behavioral Addictions, 13(2), 313–326.

4. Brailovskaia, J., Siegel, J., Precht, L.-M., Friedrichs, S., Schillack, H., & Margraf, J. (2024). *[Study on reducing non-work smartphone use and work-related outcomes]*.
