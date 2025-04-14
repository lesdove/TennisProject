# TennisProject
I volunteered to take on the task of cleaning up my Tennis Coach's Club database. Here is how I will be proposing my services to her. 

<h1>Tennis Club Database</h1>

<h2>Description</h2>
This project was designed for my Tennis coach who came to me with data management struggles. Her data is incomplete and unstructured she wants to update her emailing lists with separate skill levels and more customer metrics, marketing with merch partners, and better event targetting for clients at various skill levels. <br />


<h2>Languages and Utilities Used</h2>

- <b>Python</b> 
- <b>JSON</b>
- <b>AWS S3</b> 
- <b>DynamoDB</b>
- <b>AWS Lambda (Autonomous Function)</b> 
- <b>CLI</b>

<h2>Environment Used</h2>

- <b>AWS via Mac</b>

<h2>Project walk-through:</h2>

<p align="center"
I started by creating an IAM user for the client (my coach) and gave them admin.: <br/>
<img src="https://github.com/user-attachments/assets/f607c0b2-b536-4337-97d7-59842842aceb" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
I created an S3 bucket via CLI and added the data with club-member information:  <br/>
<img src="https://github.com/user-attachments/assets/9fc9b58a-5a33-414e-9b01-9dc1139d9b8f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://github.com/user-attachments/assets/d9e3de1d-5fce-4657-9887-7463eeee0759" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Then, I created a Table in DynamoDB to manage the data. I chose DynamoDB for its fast performance and full management services:  <br/>
<img src="https://github.com/user-attachments/assets/8d8d92be-b6cb-48f1-9a25-1ff3ebdd7a04"/>
<br />
<br />
Next, I used Lambda Function to update the events mailing list based on updates to player interest using Python Programming. Interest is listed under the item "Prod_Pref_Num" and would be updated with each event type a club member attends such as raquet demos, apparel sale, beginner mixer, or advanced liveball tournament. I would go on to program lambda to update event attendance regularly as well. The test I perfomed confired that the database is updated to reflect new event interests when new data is collected:  <br/>
<img src="https://github.com/user-attachments/assets/a180e13d-609e-485d-805a-e521bd34fd94"/>
<br />

Here is the Python Code I used to automate the database to update player interests. I would sync this to their profile based on the kinds of events they attend at the clubhouse: 
<br />
<img src="https://github.com/user-attachments/assets/1a2e8c37-3ef8-41dc-bc91-63d83bfa1698" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Lastly I performed a final test to confirm that the document from my s3 file containing the data loads into my database. This ensures that the information stored in my bucket is sent directly to the NoSQL database to be managed autonomously.:  <br/>
<img src="https://github.com/user-attachments/assets/d18f0d9d-451e-433e-87a3-490e45fba0f2" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

# Conclusions:

In this project, I organized my coach's existing data to be be stored directly into an S3 Bucket, The data is managed by DynamoDB consistently and a Lambda function was implimented to update club-member event interests. This program allows my coach to better construct mailing list for events depending on client interests. Furthermore, the autonomous function can continually update the database to add new members, update skill level and rmeove unactive members.
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
