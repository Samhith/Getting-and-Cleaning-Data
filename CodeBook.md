The five steps are perormed as follows :

1. Binding is done using the rbind() function
2. The columns with mean and standard deviation 
   measures are taken from the whole dataset.
   After that names are taken using features.txt file.
3. Activity names and IDs are taken from activity_labels.txt
4. Columns with vague names are corrected.
5. We generate a new dataset with all the average measures for each subject and activity type (30 subjects * 6 activities = 180 rows). 

The output file is called output.txt.


The following are the variables :

1.x_train, y_train, x_test, y_test, subject_train, subject_test: contain the data from the downloaded files.
2.x_data, y_data, subject_data: merge the previous datasets to further analysis.
3.features: contains the correct names for the x_data dataset, which are applied to the column names stored in  mean_and_std_features.
4.A similar approach is taken with activity names through the activities variable.\n
5.all_data merges x_data, y_data and subject_data in a big dataset.\n
6.Finally, output contains the relevant averages which will be later stored in a .txt file. 
