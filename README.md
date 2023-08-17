# NetflixMoviesAndTVShowsClustering
![download](https://github.com/saraswatiyangandul20/NetflixMoviesAndTVShowsClustering/assets/126682023/6fa642d4-f21c-4eb9-8026-9276e30b0438)


In order to maintain a top-notch user experience and mitigate subscriber attrition, it is imperative for Netflix, the global frontrunner in online streaming services boasting more than 220 million subscribers as of 2022, to proficiently categorize the content available on their platform into relevant clusters.
# Table of Content
### Problem Statement
The primary objective of this project is to conduct an analysis of the extensive collection of movies and TV shows available on Netflix. The dataset, obtained from the third-party search engine Flixable, will be subjected to clustering to categorize them into meaningful groups. This endeavor is geared towards improving user satisfaction and mitigating subscriber attrition for Netflix, the global leader in online streaming services with a subscriber base exceeding 220 million as of the second quarter of 2022. The dataset comprises content up to the year 2019, enabling the exploration of fresh insights and emerging trends within the dynamic realm of streaming entertainment.
### Objective
The aim of this project is to categorize Netflix shows into separate clusters, ensuring that shows within each cluster share similarities while also ensuring that shows in different clusters are distinctly dissimilar from one another.
### Dataset
The dataset employed in this project is obtained from Flixable, an independent search engine for Netflix content. This dataset encompasses details about every movie and TV show accessible on the streaming platform up to the year 2019. With a collection of 7787 records and 12 attributes, each attribute offers distinct information regarding the respective movie or TV show. For additional insights into the dataset, kindly refer to the Kaggle website at [(https://www.kaggle.com/datasets/sambhajizambre/netflix-movies-and-tv-shows-clustering?select=netflix_titles.csv)]
### Data Pipeline
* Understanding Your Data: The project commenced with a thorough examination of the dataset's diverse attributes. Our objective was to grasp the data's composition, structure, and potential patterns or trends. Our analysis encompassed evaluating the data's shape, discerning the data types for each attribute, and conducting a statistical overview.

* Exploratory Data Analysis (EDA): We proceeded to delve into an exploratory analysis of the data. This step aimed to unveil intricate patterns, dependencies, and insights that could fuel subsequent processing stages, thereby facilitating informed decision-making.

* Data Refinement: Rigorous steps were taken to ensure data integrity. This involved scrutinizing the dataset for instances of duplication and null values. Addressing these concerns, we tactically managed null values and even opted to eliminate specific null rows. Furthermore, any outliers were meticulously treated, enhancing data quality.

* Preprocessing of Textual Data: A comprehensive array of textual data preprocessing techniques was applied. These included removing stop words, eliminating punctuation, converting text to lowercase, stemming, tokenization, and word vectorization. In tandem, Principal Component Analysis (PCA) was employed to counteract the challenges posed by dimensionality.

* Cluster Implementation: Leveraging the efficacy of the K-Means and Agglomerative Hierarchical clustering algorithms, we orchestrated the clustering of movies. The focus was on establishing the optimal number of clusters that best encapsulated the inherent relationships within the dataset.

* Creation of Content-Based Recommendation System: A content-based recommendation system was meticulously crafted using a similarity matrix generated through cosine similarity calculations. This innovative approach empowers users with tailored recommendations, rendering ten suggestions rooted in the type of movie or show they've previously viewed.
### Project Structure

├── README.md
├── Dataset 
│   ├── [NETFLIX MOVIES AND TV SHOWS CLUSTERING.csv]()
├── Problem Statement
│
├── Understanding Data
│
├── EDA
│   ├── Numeric & Categoric features
│   ├── Univariate Analysis
│   ├── Bivariate Analysis
│   ├── Multivariate Analysis
├──Data Cleaning
│   ├── Duplicated values
│   ├── NaN/Missing values
│   ├── Treating Outlier 
│
├── Textual Data Preprocessing
│   ├── Clustering Attributes
|   ├── Removing Stopwords
|   ├── Lowercasing words
|   ├── Removing Punctuation
|   ├── Stemming
│       ├── Snowball Stemmer
|   ├── Word Vectorization
|       ├── TF-IDF (Term Frequency - Inverse Document Frequency)
|   ├── Dimenssionality Reduction
|       ├── PCA (Principle Component Analysis)
│
├── Model Building
|   ├── Clustering Implemention
|       ├── K-Means Clustering
|           ├── Elbow Method
|           ├── Silhoutte Score Analysis
|       ├── Agglomerative Hierarchical Clustering
|           ├── Dendogram
├── Content Based Recommendation System
|
│   
├── Report
├── Presentation
├── Result
└── Reference
### Conclusion
Within this project, we confronted the challenge of text clustering, aiming to categorize and organize Netflix shows into distinct clusters. Our objective was to create clusters in a manner that fosters similarity among shows within the same cluster while ensuring clear differentiation between shows situated in separate clusters.
- There were approximately 7787 records and 11 attributes in the dataset.
- We started by working on the missing values in the dataset and conducting exploratory data analysis (EDA).
- It was discovered that Netflix hosts more movies than television shows on its platform, and the total number of shows added to Netflix is expanding at an 
exponential rate. Additionally, most of the shows were made in the United States.
- The attributes were chosen as the basis for the clustering of the data: cast, country, genre, director, rating, and description The TFIDF vectorizer was 
used to tokenize, preprocess, and vectorize the values in these attributes.
- 10000 attributes in total were created by TFIDF vectorization.
- The problem of dimensionality was dealt with through the use of Principal Component Analysis (PCA). Because 3000 components were able to account for more than 
80% of the variance, the total number of components was limited to 3000.
- Utilizing the K-Means Clustering algorithm, we first constructed clusters, and the optimal number of clusters was determined to be 6. The elbow method and 
Silhouette score analysis were used to get this.
- The Agglomerative clustering algorithm was then used to create clusters, and the optimal number of clusters was determined to be 7. This was obtained after 
visualizing the dendrogram.
- The similarity matrix generated by applying cosine similarity was used to construct a content-based recommender system. The user will receive ten 
recommendations from this recommender system based on the type of show they watched.
