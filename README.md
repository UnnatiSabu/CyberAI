# CyberAI
This project aims at creating a model that classifies unstructured text into categories of complaints such as Online Financial Fraud and Cyber Attacks, sub classes of which are Fraud Call Vishing and SQL Injection. The intended outcome of this project is to automate the categorization of unstructured text, thereby aiding organizations to classify complaint data for better decision and workflows of related items.
1. Data Preprocessing:
The first step was to clean the text data for analysis through tokenization, removal of stop words, stemming, and general text cleansing.
2. Model Development
Two models have been chosen for classification
Random Forest It was applied due to its ability in handling imbalanced datasets and good processing capacity of texts that are high dimensional.
-RNNs: Used to identify sequential patterns traversing through text, which is very important in many cases where context or the arrangement of words is of significance.
3. Feature Engineering:
Feature extractions were performed on the train dataset and test dataset. Data visualization techniques such as count plots, stacked bar charts, and word clouds were used in viewing data distributions to reveal important patterns.
4. Data Processing:
Data Preprocessing techniques involved included removal of non-alphanumeric characters, null value handling and lemmatization along with sentence tokenization. Word embeddings through techniques such as Word2Vec and one-hot/label encoding for categorical variables were employed.
5. Model Training and Hyperparameter Tuning:
Random Forest
The best parameters used are the ones obtained from the hyperparameters optimized using RandomizedSearchCV with n_estimators=500, max_depth=30 and class_weight='balanced' in order to deal with imbalanced datasets better.
RNN: The model had utilized ReLU activation function, softmax output, categorical cross-entropy loss function, and Adam optimizer in training over 50 epochs.
6. Model Evaluation:
The models are evaluated by means of such performance metrics as accuracy, precision, recall, and F1-score:
Random Forest: It was able to classify the major ones successfully at about 98% while failing in subcategories with a mere 52% accuracy.
- RNN: Could have done very well on the sequenced data patterns, but was outdone by this biased dataset.
Results and Findings:
- Random Forest: Though it could achieve 98% top-level classification its efficiency in the case of secondary categorization has drastically gone down.
- RNN: Can classify sequential data but in this case has proved to be useless for the biased data. 
Implementation and Possible Improvements:
This paper provides an outline of how NLP may be leveraged for the automation of text analytics in the financial and cybersecurity industries.The model proposed here is good at main category classification, but with subcategories, it was not so good. Future studies could take techniques like XGBoost, CNN, or BERT to elevate the levels of accuracy to classify the correct subcategory.
It could feed into the organization's data pipeline using the model to classify complaints and cybersecurity incidents in real time. This streamlines processes and cuts manual intervention.
Conclusion:
This project applies NLP to some problems in financial and cybersecurity fields. Although the present model has some promising facts, it should be better tuned to keep up with both high main categories and subcategories. The advanced techniques would increase the precision of the models, making the task of classification more efficient.
