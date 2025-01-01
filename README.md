# This is Module 12, nosql-challenge.

The assignment consists of 2 jupyter notebooks located in the code folders,
a .json file used to access uk_food db. and to update the 'establishments' collection.

Part 1 uses the NoSQL_setup_starter.ipynb to show the existence of the database.
Part 2 updates the establishments collection with a new restaraunt and remove all the Dover records.
The update is done by checking for missing identity fields and update the 'BusinessTypeID'.
The removal of the Dover records is completed by using the find and determining "LocalAuthorityName"
is the key to complete the delete_many. There were 994 Dover records, all were removed and test done
confirmed all remaining records were untouched. The final portion of part 2 is to update latittude
and longitude from string to number using update_many and then to do rating value to an integer.  

Part 3 begins the use of the NoSQL_analysis_starter.ipynb located in the Code folder and loads in the
updated uk_food database from the setup_starter notebook. There are 4 pandas DataFrames made in this
excercise. I saved a .csv for each to show the outcomes of the requested exercises. In order hygiene,
rating, degree results and local authority. Utilizing the find, query and count to build the first few
dfs, took and used aggregation with match, group, sort to create a pipeline.