## John Barden Week 13 Homework
### Activity File: Exploring Kibana

* You are a DevOps professional and have set up monitoring for one of your web servers. You are collecting all sorts of web log data and it is your job to review the data regularly to make sure everything is running smoothly. 

* Today, you notice something strange in the logs and you want to take a closer look.

* Your task: Explore the web server logs to see if there's anything unusual. Specifically, you will:

:warning: **Heads Up**: These sample logs are specific to the time you view them. As such, your answers will be different from the answers provided in the solution file. 

---

### Instructions

1. Add the sample web log data to Kibana.

2. Answer the following questions:

    - In the last 7 days, how many unique visitors were located in India? <B>ANSWER: 223</B>

    - In the last 24 hours, of the visitors from China, how many were using Mac OSX? <B>ANSWER: 14</B>

    - In the last 2 days, what percentage of visitors received 404 errors? <B>ANSWER: 21</B>How about 503 errors? <B>ANSWER: 10</B>
    - In the last 7 days, what country produced the majority of the traffic on the website?<B>ANSWER: China - 280</B>
    - Of the traffic that's coming from that country, what time of day had the highest amount of activity?<B>ANSWER: 12 Noon</B>
    - List all the types of downloaded files that have been identified for the last 7 days, along with a short description of each file type (use Google if you aren't sure about a particular file type).</br> <B>ANSWER:</br>gz - Compressed archive vile</br>css - Cascading Style Sheet file</br>zip - compressed archvie file</br>deb - debian software package file</br>rpm - Red Hat Package manager file </B>

3. Now that you have a feel for the data, Let's dive a bit deeper. Look at the chart that shows Unique Visitors Vs. Average Bytes.
     - Locate the time frame in the last 7 days with the most amount of bytes (activity). 
     - In your own words, is there anything that seems potentially strange about this activity?<B>ANSWER: There was a significant number of Bytes associated with a single unique visitor</B>

4. Filter the data by this event.
     - What is the timestamp for this event?<B>ANSWER: 11/28/21 @ 9:00PM</B>
     - What kind of file was downloaded?<B>ANSWER: rpm - Red Hat Package Manager File</B>
     - From what country did this activity originate? <B>ANSWER: IN - India</B>
     - What HTTP response codes were encountered by this visitor? <B>ANSWER: 200 OK</B>

5. Switch to the Kibana Discover page to see more details about this activity.
     - What is the source IP address of this activity? <B>ANSWER: 35.143.166.159</B>
     - What are the geo coordinates of this activity?<B>ANSWER: lat 43.34121, lon -73.6103075 </B>
     - What OS was the source machine running? <B>ANSWER: Windows 8 </B>
     - What is the full URL that was accessed? <B>ANSWER: https://artifacts.elastic.co/downloads/beats/metricbeat/metricbeat-6.3.2-i686.rpm</B>
     - From what website did the visitor's traffic originate? 	<B>ANSWER: http://facebook.com/success/jay-c-buckey</B>

6. Finish your investigation with a short overview of your insights. 

     - What do you think the user was doing? <B>ANSWER: The user was downloading the metricbeat package for debian</B>
     - Was the file they downloaded malicious? <B>ANSWER:No, this does not appear to be malicious </B>If not, what is the file used for? <B>ANSWER:This file is used to configure metricbeat on a web server </B>
     - Is there anything that seems suspicious about this activity? <B>ANSWER: Only that the link for metricbeat package was on someone's facebook page</B>
     - Is any of the traffic you inspected potentially outside of compliance guidlines? <B>ANSWER: If facebook.com/success/jay-c-buckey is not a trusted source, then this potentially is out of compliance allowing the user to download files linked from this server.</B>

---
?? 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.  
