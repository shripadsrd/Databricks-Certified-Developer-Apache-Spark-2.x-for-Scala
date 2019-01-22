# Databricks Certified Developer – Apache Spark 2.x for Scala

After about a year of learning Apache Spark and writing Spark applications, I decided to get certified by Databricks in August this year. After preparing on and off for a few months after, I was finally able to obtain this certification in December of 2018.

Upon updating my LinkedIn profile to reflect the certification, a few people reached out to me asking for details about the test. So, here I am, sharing my experience of preparing and taking the test:

### Why bother with Apache Spark?

I have been working with Apache Hadoop and Apache Spark for Data Processing for some years now, and have also had the opportunity to work with Spark on a few POCs and migration projects. Apache Spark has always been in the news with its claims of being the fastest data processing engine. And while there have been newer engines that claim to do more, Spark seems to be a mature project with good backing from Databricks and a very good community of Committers. Spark also seems to be improving quickly: the initial release was in 2014, but as of December 2018, it is on version 2.4.0 and has evolved rapidly. According to Databricks, “Spark has one of the largest open-source communities in Big Data, with over 1000 contributors from 250+ organizations.” Apache Spark is 100 times faster than Hadoop, it’s very easy to learn, it provides a great stack of libraries for various use cases and it can run on multiple types of clusters which makes migrating to Spark a very easy process. Several companies are using Spark as their Big Data processing engine now, which also makes it an attractive skill to learn for potential job applicants.

### Why bother with the certification?

According to Databricks, “Databricks Certification validates your overall knowledge on Apache Spark and assures employers that you are up-to-date with the fast-moving Apache project, with significant features and enhancements being rolled out rapidly [1].” There are other vendors like Hortonworks and Cloudera who also have their own certifications, but because Databricks is deeply involved in developing Spark, their certification seemed the most attractive to me.

If you are a Spark Committer, there is no reason for you to take the test. I wanted to learn Spark, and for me personally, a tangible end goal such as a test was much needed motivation. The Databricks certification for Spark tests your knowledge in depth and on all the important aspects of Spark. So, to clear the test, you will need to go looking for information and understand all aspects of it rather than focusing only on what you care about.

The certification also is a nice feather to have in your hat and lets you show off your Spark knowledge on your resume.

### Ok, great! How do I get started?

Before you start studying Spark, you need to figure out what language you are going to be using Spark with. You can write Spark applications in Java, Scala, or Python (also SQL and R), although the test is only available with Scala or Python. Spark APIs are consistent across languages in terms of speed and stability. I chose Scala because Spark is written in Scala; and in some cases, Scala can be faster than Python. However, if you do not know Scala or Python, Don’t Panic! You need to learn just enough Scala to be able to run Spark code, which is not a lot. I recommend reading “Programming in Scala” by Bill Venners and Martin Odersky [4] for the same.

I started learning Spark by reading the book “Spark: The Definitive Guide” by Bill Chambers and Matei Zaharia [2]. This book is easily the best resource you can use to start learning about Spark. Before Spark 2 came along, I had read the book “Learning Spark” by Holden Karau, Andy Konwinski, Patrick Wendell, & Matei Zaharia [3], which is a great book, but it is also outdated and unnecessary for the test (or for learning Apache Spark in general). After completing this book, I went through Programming Guides for RDD [5], Spark SQL [6] and Structured Streaming [7]. These links are (as of Dec 2018) the same as the material in the book, but as newer versions of Spark are released, expect to see updated information on the Programming Guides. Databricks Blogs [8] and SAIS videos [9] are also great places to keep yourself informed about developments in Spark. I have also added a few URLs towards the end of this article, which I highly recommend; some videos/documents may be from Spark 1.0, but they are still relevant and going through them will possibly help connect a few dots in your mind.

If you have worked on Map-Reduce applications before, Spark should be very easy to understand. If you have never worked on Spark or have no experience building distributed applications, you might want to work on a few projects or take an online course on Apache Spark. I recommend the course “Apache Spark 2 with Scala” by Frank Kane on Udemy [10].

If you don’t mind spending some money, you can also take a self-paced course on Databricks Academy [11]; this course is good at explaining DataFrames and you also get to work on exercises. However, if you read the Programming Guides properly and practice a few examples with sample data, you don’t have to spend any money on it.

If you are willing to spend more money on this, or if you can get your employer to sponsor it, you can also consider attending the Spark AI Summit 2019 in San Francisco [12]; they have instructor-led training sessions at the conference.

There are, currently, no “dumps” available for this test online. This, in my opinion, is a good thing and I hope it stays this way.

### Tell me more about the test.

You can take a live proctored test at home, or you can take the test online. The cost of taking the test is $300, this gives you two attempts at clearing it. Check Databricks Academy for more information [13].

The test is 180 minutes long and has 40 questions. You need to score at least 65% (get 26 questions correct) to pass the test.

### Can you give me any tips?

* Yes, I won’t give you a list of questions I was asked, but here are a few things to keep in mind:
* Don’t forget about RDDs. Even though the test says Spark 2.x, RDDs are an important part of the Spark engine. There may not be many questions about RDDs, but * understanding what they are and how they work is very important. Expect at least 2 questions on RDDs.
* It is important to understand how and when Spark shuffles data. Shuffles are expensive; keep your transformations narrow.
* Know your transformations from your actions.
* UDFs and UDAFs are important.
* Know how to read from and write data to various sources and sinks using Apache Spark; pay attention to the syntax and options.
* Expect one question on GraphFrames [14].
* Expect one question on Spark MLLib.
* Find out what Encoder, Tungsten, and Catalyst do.

I hope you enjoy learning Apache Spark, and I wish you all good luck with your test. Please leave a comment or reach out to me if you have questions or suggestions.

### References
[1] https://databricks.com/training/certified-spark-developer

[2] https://www.amazon.com/Spark-Definitive-Guide-Processing-Simple/dp/1491912219

[3] https://www.amazon.com/Learning-Spark-Lightning-Fast-Data-Analysis/dp/1449358624

[4] https://www.amazon.com/Programming-Scala-Updated-2-12/dp/0981531687/

[5] https://spark.apache.org/docs/latest/rdd-programming-guide.html

[6] https://spark.apache.org/docs/latest/sql-programming-guide.html

[7] https://spark.apache.org/docs/latest/structured-streaming-programming-guide.html

[8] https://databricks.com/blog/category/engineering/spark

[9] https://databricks.com/sparkaisummit/north-america/sessions

[10] https://www.udemy.com/apache-spark-with-scala-hands-on-with-big-data/

[11] https://academy.databricks.com/products/dataframes

[12] https://databricks.com/sparkaisummit/north-america

[13] https://databricks.com/training/certified-spark-developer/how-to-take-the-exam

[14] https://databricks.com/blog/2016/03/03/introducing-graphframes.html

### Miscellaneous links:
https://graphframes.github.io/user-guide.html

https://databricks.com/blog/2015/04/13/deep-dive-into-spark-sqls-catalyst-optimizer.html

https://community.hortonworks.com/articles/72502/what-is-tungsten-for-apache-spark.html

https://academy.databricks.com/products/dataframes

https://www.youtube.com/watch?v=7ooZ4S7Ay6Y

https://www.youtube.com/watch?v=1a4pgYzeFwE

https://www.youtube.com/watch?v=rl8dIzTpxrI

https://databricks.com/blog/2016/08/15/how-to-use-sparksession-in-apache-spark-2-0.html

https://databricks.com/blog/2016/01/04/introducing-apache-spark-datasets.html

https://databricks.com/blog/2016/07/14/a-tale-of-three-apache-spark-apis-rdds-dataframes-and-datasets.html

https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/8599738367597028/1499152197856461/3601578643761083/latest.html

http://cdn2.hubspot.net/hubfs/438089/notebooks/spark2.0/SparkSessionZipsExample.html

https://github.com/vaquarkhan/vk-wiki-notes/wiki/Apache-Spark-Join-guidelines-and-Performance-tuning
