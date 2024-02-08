
# list all the files 
ls -ltr 

# list all the files in hadoop 
hadoop fs -ls /

# create new folder in hadoop 

hadoop fs -mkdir /tmp/input_data


# move data into hadoop folder 
hadoop fs -put movies.csv /tmp/input_data
hadoop fs -put ratings.csv /tmp/input_data
hadoop fs -put tags.csv /tmp/input_data

hadoop fs -put user_profile_data.json /tmp/input_data
hadoop fs -put store_data.json /tmp/input_data
hadoop fs -put ad_campaigns_data.json /tmp/input_data

# list  the file in the hdfs folder 
hadoop fs -ls /tmp/input_data 