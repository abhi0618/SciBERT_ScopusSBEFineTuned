# SciBERT_ScopusSBEFineTuned

This Code was executed on Google Coolab,and all the necessary files for tokenization,training and inference were uploaded to a google drive to link the data to the Collab scripts.It is advised to download and then upload all the contents in a new personal google drive folder, to avoid any permission issues.

For the 1st part of the code, please upload the scopusjournalall.xlsx file  to the the current environment content, meaning you would have to upload the file again to  the script after disconnecting and rerunning the runtime script.

For the second script Language Modelling, the script takes the pre_train.txt file from the 1st file's output as its input in the second script.This step takes up quite a bit of time and memory,and hence is recommended to use collab's GPU in  the processing.

For the 3rd script , upload  the Sciee training dataset along with our custom training and testing datasets,to the session content folder.The training model,pytorch and weights are taken from the best result producing  checkpoint from the 2nd step of Language Modelling .

Altough the scripts require external packages , collab mostly has them preinstalled, except the transformers and the simpletransformers package,that we have to intall,along with the pytorch packages.

There are no path modifications to be done in the 4th and the 5th files, as the 4th file reads the eexcel file , making predictions of entitites on each row and then saving the predictions in a pickle file. The final script appends the predctions to a new column in the excel file and saves it as the Final.csv File.
