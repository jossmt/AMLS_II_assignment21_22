# README

## Project Outline
The code for both tasks is contained in a single jupyter notebook. The notebook proceeds to:

1. Read the datasets depending on the task variable set (A or B)
2. Sample different sentiment classifications with equal distribution (positive/negative/neutral)
3. Pre-Process the text by removing @ values and stripping white space
4. Tokenize the data using BERT tokenizer
5. Split the data into batches for each of train/test/validation to be iteratively executed
6. For each iteration of the BertClassifier model we: transforming the feature vector using BERTModel, feeding forward the feature vector through the neural network, backpropagating the loss function and finally storing the results for every 10 batches.
7. Visualise the training loss and validation accuracy before evaluating the test dataset against the final model. 

## Execution
The model can be executed by running the notebook in Google Colab (ensure to upload the competition data to the same directory as the notebook). In order to run task A simply execute the notebook with task parameter set to 'A', otherwise set the task parameter to 'B' to run the model for task B. The results of the most recent run for Task B can be seen in the notebook results. 

###### Note: The model was unfortunately built using jupyter notebooks in google colab and the results were re-run at the final hour, so the model has not been transformed into an executable python script in time. 
