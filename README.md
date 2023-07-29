# Data Extraction, Transformation and Loading (ETL)

This involves extraction of 1000s of CSV files whose data is to be transformed to time series. Each file belongs to one of the six different sources termed as OLT.
The output consists of six csv files with timeseries data, each for one OLT

Below is the format of each CSV file
Each column entry has three counter values separated by a comma(,) and counts are taken in intervals of 5 minutes apart. The start time is in the first 4 rows of the file which describe the dataset, they represent the header of the CSV file.

The arrangement of the header is different from that of the real data in the file.

The code here was to wrangle every file into a desired format and concatenate all the files from the same OLT into one timeseries csv file with the use of python
