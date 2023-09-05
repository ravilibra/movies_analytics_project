# Hello..! I'm Ravi Kumar (Data Engineer)
🔭 I’m currently working on Movie analytics Project

👨‍💻 All of my projects are available at 

📝 I regularly write articles on [Data engineering tech stack](Data engineering tech stack)

📫 How to reach me dksidd96@gmail.com

onnect with me:


Languages and Tools:
docker hadoop hive pandas python

Table of contents
General info
Technologies
Architecture
Setup
General info
This project is about Movie Analytics.

Technologies
Project is created with:

Hadoop
Hive
Spark


image

Detailed Explanation: For this project there are 3 data sources named as ratings.csv,users.csv,movies.csv. In the ratings.csv there are 4 columns userid , movieid , rating, timestamp. The userid gives the detail about the user,the movieid gives the information of the movie to which user gave rating. The rating will be in between 1 to 5. In the users.csv we have 4 columns userid,gender,occupation,zip-code.The userid gives information about the user.the gender gives information regarding the gender of the user and the occupation gives the info regarding occupation of the user and zipcode gives the information about the zipcode of the user. In the movies.csv we have 3 columns. we have information regarding movieid,title genre.the moviid gives the id of the movie,the title represents the title for the movieand genre gives the information regarding to which genre it belongs to this columnis again delimted by ‘|’.it has various values in that column like action, Thriller etc.

Our data is picked from the hdfs layer and read by the spark engine. After reading the data We can perform various analytical queries on the data and extract useful business insights like top 10 viewed movies,distinct list of genres,to which genre audience are giving more ratings etc.So that the movie industry can analyze the trends and can know the audience interests. Storage: Finally we can store the data as table in hive meatstore if required we can also create real time dashboards by using some dashboarding tools.

Setup
To run this project, install it locally: first copy all files from local to HDFS location

$ hdfs dfs -put users.csv /
$ hdfs dfs -put movies.csv /
$ hdfs dfs -put ratings.csv /
Then on the Spark shell run the below command from CLI

$ Python main.py
or
$ spark-submit main.py
Python
