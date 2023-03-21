# Final_Project_01

Title : Data Migration and Transformation Tool for Amazon RDS Data Warehouses

Goal: Extraction of the data from a zip file that is available at a URL and uploading it into Amazon S3 and Amazon RDS.

Technologies used: Python, Requests library, Zipfile library, boto3 library, psycopg2 library pandas, Amazon S3, Amazon RDS

Steps:
1.	Using Python libraries like [requests, urlib, wget, curl] to download the zip file from the URL. 
2.	Zipfile library in Python to extract the data from the zip file. This will create a file or directory containing the extracted data.
3.	AWS SDK for Python (Boto3) to create an S3 bucket.
4.	Using put_object function of Boto3 to upload the extracted data to the S3 bucket.
5.	Boto3 is used to create an RDS instance.
6.	Using psycopg2 library in Python to connect to the RDS instance.
7.	Using pandas library in Python to read the extracted data into a DataFrame and this data is pushed to RDS instance.

The above steps as code are given in the file "establishing connection betweeen S3 and RDS" 

Issues faced while doing the project:
The zip file downloaded from the given URL was not accessible and it had badzip file error. More over the URL was giving a 403 forbidden error. Hence the zip file was downloaded manually to the local system and only 50 files were uploaded into the s3 from the local system to check the code and complete the project.

The same as code is given in the file "establihing connection between loacl and S3"


