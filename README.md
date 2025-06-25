# Setup Guide and General Information
This is the updated natural language processing. I will address all the ten revisions here in Read Me. The documentation is mainly about the set up and content of the natural language processing, and is also updated. Please download this zip and run all the cells. I have included the entire project, not only the updated section.

# Download File
Please also download the "output" folder and the "bert LLM Natural Language Processing" folder at https://www.mediafire.com/folder/tmtou63yyo0dm/BERT_statistical_model. The file size is 1 GB. Then, please put these two folders in the zip folder, the same location as the Jupyter Notebook. If you want, you could choose to not download the file. The main reason for download is that you don't have to wait to train the natural language processing model. Please see the "Updated Statistical Model" section in the Jupyter Notebook for detail.

# Revision

## Revision 1: What are the risks of assigning fixed cutoff values for sentiment (positive, negative, neutral) without justification?
If utilizing multiple statistical models, the same threshold is not suitable for all the statistical models. Each statistical model is likely to have different loss function, and different sigmoid function. Some even have different algorithm other than crosss entropy (such as utilizing binary cross entropy). Thus, is important to compute threshold for different statistical models. In this project, I compute threshold for the Review Classifier statistical model (utilized in the last version), the updated BERT model includes built in threshold. In this way, different thresholds are computed for different statistical models.

## Revision 2: Why is it problematic to rely on only one open-source tool like TextBlob for sentiment analysis?
Different statistical model is more suitable for different data set and different classification computation. Statistical models that utilize binary cross entropy are more suitable for binary classification (although recently there are studies that incorporate binary cross entropy for other classification), MSE are more suitable for linear regression. In this project, for supervised learning, I add BERT and compute the data set with BERT; I find that BERT is more accurate than Review Classifier statistical model. For unsupervised learning, I add vader, and the rating is also more accurate. For prediction, I add BERT prediction and find more accurate predictions.

## Revision 3: Why does a well-made chart still fall short without an interpretation?
A visualization sometimes may include many things, or is hard to understand. Thus, including caption could explain the visualization better. In this project, I have created additional visualizations for BERT and add captions to all visualization to explain the data in more detail.

## Revision 4: What issues arise from inventing metrics without a clear rationale?
Each metric should be rational and reasonal. If not, then the statistical model could be wrong. In this project, I have research and study natural language processing and unsupervised learning a lot, and make suer every metric is rational.

## Revision 5: What are the dangers of letting AI tools drive the entire analysis?
AI, in the end, is a py file. AI is not, and never will be, a human who possesses the ability to actually feel the emotion of other people. Thus, we should always unit test the result. In this project, I have read the resulted data (the "data" DataFrame in the project) in details (approximately 300 rows) to unit test the result.

## Revision 6: Why should feature selection in predictive modelling be thoughtful rather than automatic?
If a feature is unrelated, then it's not usefule to include this feature in the statistical model. In the project, I have constructed features according to the relatibility, and confirmed the usefulness to the statistiacl model. 

## Revision 7: Why isn’t printing R² and MSE enough in model evaluation?
First of all, R² and MSE are for regression analysis (in another world, when the amount of classifying labels is one). In classification problem (when the amount of classifying labels are two or more), accuracy is the main evaluation process. In this project, I have create custom functions for every statistical model to print the accuracy and speed up the evaluation process.

## Revision 8: Why is cross-verifying AI-generated outputs essential in analysis?
Again, in the end, AI is just a py file. Raw data is the true information. If AI's result is not the same as raw data, then is AI that's wrong. In this project, I have read the raw data extensively to confirm and unit test the result.

## Revision 9: What makes analysis more than just charts and models?
The project should guide the reader step by step to explain the computation. In this project, I have provided easy step by step explanation that simplifies the code by omitting the complex implementation and only presenting the interface, so that the reader can understand better and learn more.

## Revision 10: How can you use AI as a tool without losing your own analytical thinking?
The key is the mindset of "don't assume that AI is always right." With this in mind, people could keep critical thinking skill and study better.

# Read Me Task

## Read Me Task 1
The top three positive employees (across all the months) are lydia.delgado@enron.com, john.arnold@enron.com, and eric.bass@enron.com. The negative are kayne.coulter@enron.com, rhonda.denton@enron.com, and sally.beck@enron.com.

## Read Me Task 2
As of 12/31/2011, in the past 30 days, there's no list of employees having flight risks.

## Read Me Task 3
One of the insight I gain in this natural language processing project is that tokenizing both the email subject and content is better than only content. The statistical learning model are more accurate in this way. In addition, frequently browse the github development page of the python module that one uses, so that one could better understand and solve issues when encounter, and also have a better overall understanding of the knowledge.

# Some Personal Message from the Submitter of this Project
Thank you so much for giving me a chance to update this project. I really learned a lot, both during construction and updating. I still know that my answers may not be correct, and that there's many rooms for improvement. I will still spend time and effort the same way and more in the future. In the end, no matter whether I pass or not, thank you for your time.
