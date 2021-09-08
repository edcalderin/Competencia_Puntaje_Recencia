# Keyword Recency Score Competition

Thanks to DatasourceAI (https://www.datasource.ai/) for this opportunity.  

__Hardware used:__
Intel Core I7 Inside 2.60GHz, 8GB Ram, NVIDIA GEFORCE GTX (But it was not used in the notebook).
 
__Operative System:__ Windows 10 Home

__How to train your model?__  
You just need execute the cells from start to process and transform the necessary data. You must not execute "Training for validation" section since it was created only for competition purposes. "Training with full data" section is right if you want to train the model with entire dataset.
You have the possibility to used train processed dataset to avoid waiting for tokenization.

__How to make predictions on a new test set?__ 
- In "Predictions" Section you will can find the steps to make predictions, there are data processing again but the only difference is reduction of code lines hence It uses sklearn objects for transformations which have been already trained before.
- Tokenization process is carried out with Abstract and Title columns of test dataset, because it uses the same function for tokekinizing.
- The name of new columns must be equal to ones used in training processing step, because they will be removed using a list of strings containing these column names.
- Vectorizer of text and Post tags use the model created previously to transform the tokenized text.
- This is the pipeline to create a new prediction.
- Also, you can use test processed to make predictions jumping all previuous steps.  

__Important side effects of code:__  
Data processing code just overwrites column Year.

__Key assumptions of your code:__  
Train and Test csv files must be in same folder that notebook.
