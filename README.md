# Hack_the_feed
I began by consolidating four datasets—Twitter, LinkedIn, Instagram, and Facebook—into a single dataframe. Following this, I streamlined the dataset by eliminating irrelevant columns such as 'Link,' 'Post ID,' and 'Post Type.' Moving on to data assessment, I scrutinized column information to identify any discrepancies in data types, missing values, or inaccuracies in labels. Examining unique values in each column allowed me to detect potential inconsistencies.

Subsequently, I initiated the data cleaning process. Special characters in relevant columns were removed, and incorrect data types were rectified. To simplify handling missing values, columns with '0' and 'NaN' as their only values were replaced entirely with '0.' Employing the KNN imputer addressed numerical feature gaps, while 'unknown' replaced 'NaN' in categorical data. Duplicate rows and columns were eliminated, and the statistical behavior of the data unveiled outliers.

With the data now cleansed, I delved into Exploratory Data Analysis (EDA). Multiple insights, including engagement, content, Click-Through Rate (CTR), impression, and reach analyses, were examined. This comprehensive exploration provided a robust understanding of the dataset.

Text preprocessing followed for post analysis, involving tokenization, removal of stopwords and special characters, and lemmatization. Word clouds were generated for both post and tags features to visually represent textual patterns.

Transitioning to machine learning for impression prediction, I undertook preprocessing steps such as encoding, rescaling, standardization, and normalization. Feature selection narrowed down the model to 10 key features out of the initial 147. Rigorous testing revealed that the Ridge algorithm performed optimally, yielding a mean absolute error of 0.67.
