# ONT-Capacity-Visualization

Title: Visualizing capacity utilization of ONTs.
Objective: To graph the capacity utilization on every ONT.
The utilization of ONTs(access point in the GPON technology) can not be graphed using cacti graphing tool. After consultations with the vendor, the possible way to achieve this is to use the data collected by the Statistics and Data Collector (SDC).
The collected data is stored in CSV files. 
Every row represents an ONT
Each column entry has three counter values separated by a comma(,) and counts are taken in intervals of 5 minutes apart. The start time is in the first 4 rows of the file which describe the dataset, they represent the header of the CSV file.
The arrange ment of the header is different from that of the real data in the file.
The code here was to wrangle every file into a desired format and concatenate all the files from the same OLT into one timeseries csv file with the use of python
