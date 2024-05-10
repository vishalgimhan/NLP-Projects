# NLP-Projects

**01. Covid-19 Vaccine Sentiment Analysis**

- **Library Imports**: The notebook begins by importing various libraries for data processing, visualization, and natural language processing, such as numpy, pandas, matplotlib, seaborn, plotly, and nltk.

- **Data Preprocessing**: It includes steps to clean the text data from the dataset, such as converting text to lowercase, removing Twitter handles, hashtags, URLs, special characters, and single characters, and substituting multiple spaces with a single space.

- **Sentiment Analysis**: Utilizes the nltk library’s SentimentIntensityAnalyzer to calculate sentiment scores for the tweets, which are then used to create new columns for positive, neutral, and negative sentiments.

- **Exploratory Data Analysis**: The notebook performs exploratory data analysis (EDA) to understand the distribution of sentiments across tweets and visualizes the most common words in positive and negative tweets using word clouds.

**02. Twitter Sentiment Analysis**

- **Installation & Setup**: The notebook begins with instructions to install the Kaggle library, set up the Kaggle API, and handle the kaggle.json file. 

- **Data Handling**: It involves downloading the Sentiment140 dataset from Kaggle, extracting it, and loading it into a pandas DataFrame. The dataset is then preprocessed, including resampling to balance the classes and text processing for stemming.

- **Model Training**: A Logistic Regression model is trained using TfidfVectorizer for text data transformation. The model achieves an accuracy of 85.64% on training data and 74.48% on test data.

- **Model Utilization**: The trained model is saved and loaded for making predictions. An example is shown where a new tweet is classified as a positive sentiment.

**03. Hotel Recommendation System**

- **Library Imports**: The notebook begins by importing necessary libraries such as nltk, numpy, pandas, and specific modules for text processing like stopwords, word_tokenize, and WordNetLemmatizer.

- **Data Preparation**: It involves loading a dataset of hotel reviews, modifying the column to replace abbreviations of Countries, and extracting the country names from Text into a new ‘countries’ column. Unnecessary columns are dropped to streamline the data.

- **Data Processing**: Columns that contain string representations of lists, are converted into actual lists using the literal_eval function. The entries are then transformed to lowercase for uniformity.

- **Hotel Recommendation Function**: A function recommend_hotel is defined to recommend hotels based on a given location and description. It processes the description to remove stopwords and lemmatize the words, then compares these with the hotel tags to find similarities and ranks the hotels accordingly.
