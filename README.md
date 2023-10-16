# NLP_Sentiment_Topic

### **Objective**
Conduct sentiment analysis on a dataset of qualitative responses, extract the sentiment of each response using multiple models (NLTK, BERT, Roberta), and apply topic modeling on the responses to identify the main topics.

### **Steps**

1. **Imports**:
    - _Standard Libraries_: pandas, numpy.
    - _Visualization_: matplotlib.
    - _NLP Tools_: NLTK, transformers.
    - _Topic Modeling_: BERTopic.

2. **Data Loading**:
    - Locate the current working directory.
    - Import datasets from `.xlsx` files.

3. **Data Preprocessing**:
    - Melt (or unpivot) dataframes for easier analysis.
    - Concatenate datasets.
    - Sentence segmentation for each response.

4. **Sentiment Analysis**:
    - Use NLTK's VADER SentimentIntensityAnalyzer.
    - Use BERT model from `nlptown`.
    - Use Roberta model from `cardiffnlp`.

5. **Model Evaluation**:
    - Use a manually labeled dataset to evaluate the predictions.
    - Generate confusion matrices and classification reports for NLTK, BERT, Roberta, and an aggregated model.

6. **Model Improvement**:
    - Refine Roberta's predictions using certain indicative words.
  
7. **Final Data Preparation**:
    - Apply corrections to the dataset.
    - Extract and examine short responses.

8. **Topic Modeling**:
    - Use BERTopic to cluster responses.
    - Extract keywords for each topic.
    - Classify responses based on topic.
    - Save results in an `.xlsx` file.

9. **Output**:
    - Save processed responses in 'all_qual_responses.xlsx'.

### **Note**:
Before executing the script, make sure all dependencies are installed and datasets are in the working directory. This README provides an overview. Deep domain knowledge might be required to modify or fully comprehend the script.
