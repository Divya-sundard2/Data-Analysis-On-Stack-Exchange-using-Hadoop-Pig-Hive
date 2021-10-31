# Data-Analysis-On-Stack-Exchange-using-Hadoop-Pig-Hive
**Task1:Acquiring data from stack exchange database**
The Data was acquired from stack exchange database by using its Application Programming Interface (API) with the help of SQL query. The task which was assigned to me to acquire the top 2,00,000 posts which has highest view count. Posts is the table which has all the necessary information about posts like view count, owner, title of the posts etc.
I can download 50,000 records as CSV file in a single shot. I can fetch top 2,00,000 records by using SQL

**Task2:Load amd query the output**
From this link I performed loading CSV using CSVExternalStorage,So I downloaded the piggybank.jar from http://www.java2s.com/example/jar/p/download-piggybank0120jar-file.html  to use csv loader() function in pig. This function helps us to load all the csv files. I loaded all my csv files into pig by using commands which is uploaded inside Load data into pig 
after loading we have to store the data inside pig.

**Task3:**
for all these tasks we hace to create a table to store the data and perform RDBMS operations.
(i) Query to find top10 posts by score
(ii)Query to find top 10 users by post score
(iii)The distinct number of users who used the word "cloud" in one of their posts

TASK4:
Using hivemall-core we are going to find TF-IDF for top 10 terms for the top 10 users

for this we need to download the https://github.com/myui/hivemall/releases/download/v0.4.2-rc.2/hivemall-core-0.4.2-rc.2-with-dependencies.jar. using** wget** command
We have to define the hive refernced from https://github.com/apache/incubator-hivemall/blob/master/resources/ddl/define-all-as-permanent.hive.

We can find top 10 users by post and we can find the top 10 terms by calculating TF_IDF for the terms,we have to make temporary table or view to map the terms score and the users


All the four tasks are implemented by using Google dataproc cluster


References:**https://data.stackexchange.com/stackoverflow/query/new**
             **https://github.com/kirthy21/Data-Analysis-Stack-Exchange-Hadoop-Pig-Hive-MapReduce-TFIDF** referred for loading and storing into pig as hdfs path
             **https://github-wiki-see.page/m/daijyc/hivemall/wiki/TFIDF-calculation**
             **https://github.com/rajesh-codes/Stack-Exchange-Data-Analysis** made some modificatopns accoding to my table name and  view name to find TF-IDF
             
