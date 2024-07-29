# Automated-Essay-Scoring
Automated Essay Scoring on The Hewlett Foundation dataset on Kaggle

Automated essay scoring (AES) uses specialized computer programs to assign grades to essays written in an educational setting. It is a form of educational assessment and an application of natural language processing. Its objective is to classify a large set of textual entities into a small number of discrete categories, corresponding to the possible grades, for example, the numbers 1 to 6. Therefore, it can be considered a problem of statistical classification. Automated essay scoring (AES), the task of employing computer technology to score written text, is one of the most important educational applications of natural language processing (NLP). <br><br>
This area of research began with Page’s [1966] pioneering work on the Project Essay Grader system and has remained active since then. The vast majority of work on AES has focused on holistic scoring, which summarizes the quality of an essay with a single score. There are at least two reasons for this focus. First, corpora manually annotated with holistic scores are publicly available, facilitating the development of learning-based holistic scoring engines. Second, holistic scoring technologies are commercially valuable: being able to automate the scoring of the millions of essays written for standardized aptitude tests such as the SAT and the GRE every year can save a lot of manual grading effort <br><br>
<b>Data Collection: </b><br>
In this step, the raw essay data is collected from various sources over the internet (Kaggle, google dataset), we also conducted a small survey among the children who were aged between 10-15 over varied essay topics to get better data in the community. We also contacted our mentor who helped us mention the online sources like pdfs of authors that can be used for the purpose of data collection. The data is also normalized by converting all the text to lowercase and removing any extra spaces.
<br>
<br>
<b>Tokenization:</b><br>
IndicNLP This step involves breaking down the essays into individual words or tokens. Tokenization is important because it helps to create a structured representation of the essays that can be used for analysis.
Stopword Removal: In this step, commonly used words that do not carry much meaning, such as "a," "an," and "the," are removed from the essays. This helps to reduce the noise in the data and improve the accuracy of the system.
Stemming/Lemmatization: This step involves reducing words to their base or root form. For example, "running" and "ran" would both be reduced to "run." Stemming or lemmatization helps to reduce the dimensionality of the data and improve the accuracy of the system.
<br>
<br>
<b>Feature Extraction:</b><br> In this step, relevant features are extracted from the preprocessed data. This can be done using various techniques such as Bag-of-Words (BoW), n-grams, or Word Embeddings. The goal of feature extraction is to represent the essays in a format that can be easily analyzed by machine learning algorithms.
<br>
<br>
<b>Data Splitting:</b><br> In this step, the preprocessed data is split into training, validation, and testing sets. The training set is used to train the machine learning model, the validation set is used to tune the hyperparameters of the model, and the testing set is used to evaluate the performance of the model.
<br>
<br>
<b>Model Selection:</b><br> For this project, I had chosen Gradient Boosting Regressor over various Regression algorithms like SVM, Linear Regression, and Neural network because Gradient Boosting regression suited our data, since it was regional data there were a high number of outlier data as well as the neural network had a high computation time. This made it complicated to use. The data doesn’t have complicated input values in them.  GBR provides interpretable results, making it easy to understand how each feature contributes to the final prediction. In contrast, NN can be difficult to interpret.
<br>
<br>
Gradient Boosting Regressor is an ensemble-based algorithm that combines the predictions of multiple weak models to make a final prediction. This allows it to achieve high accuracy in AEG systems, especially when combined with appropriate feature engineering techniques. It is a flexible algorithm that can be tuned using various hyperparameters, such as the learning rate, number of trees, and depth of each tree. This flexibility allows it to adapt to different AEG scenarios and achieve high accuracy.
<br>
<br>

