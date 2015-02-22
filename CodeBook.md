The script run_analysis.R performs the 5 steps described in the course project's definition.

1. First, similar data from training and test is merged using rbind() function
2. Then, only those columns with the mean and standard deviation measures are taken from the whole dataset. After extracting these columns, they are given the correct names, taken from features.txt.
3. Activity names and IDs from activity_labels.txt are referenced and substituted in the dataset.
4. On the whole dataset, those columns with vague column names are corrected.
5. Finally, a new dataset with all the average measures for each subject and activity type is generated. The output file is called averageData.txt, and uploaded to this repository.

Variables

1. "x_train", "y_train", "x_test", "y_test", "subject_train" and "subject_test" contain the data from the downloaded files.
2. "x_data", "y_data" and "subject_data" merge the previous datasets to further analysis.
3. "all_data" merges "x_data", "y_data" and "subject_data" in a big dataset.
4. "averageData" contains the relevant averages which will be later stored in "averageData.txt" file.
