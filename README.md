# AWS Three-tier and Data Analytics Architecture

### Frontend Tier
**Amazon S3:** Host the static content (HTML, CSS, JavaScript) for the website. Enable website hosting on the S3 bucket to serve the frontend files.

**Amazon CloudFront:** Configure a CloudFront distribution to provide global content delivery with low latency and high transfer speeds. Set up the CloudFront distribution with the S3 bucket as the origin.
### Backend Tier

**Amazon EC2:** Launch EC2 instances to run the Java application and Apache Web Server. Install and configure Apache Web Server on the EC2 instances to handle incoming requests.
### Database Tier

Amazon RDS: Create an RDS MySQL database instance to store and manage the application's data. Configure security groups to allow access from the backend tier and restrict access from the internet.
### Analytics Workload

**Amazon EMR:** Set up an EMR cluster to run the Apache Hadoop-based analytics workload. Upload the data to be analyzed to Amazon S3, and configure the EMR cluster to read the data from S3. Install and configure Apache Hadoop and related tools on the EMR cluster to process and analyze the data.

**Amazon QuickSight:** Use QuickSight, a visualization tool, to create interactive dashboards and visualizations based on the analyzed data. Connect QuickSight to the output of the analytics workload running on EMR.
### Additional Services

**Amazon VPC:** Create a VPC to isolate and secure the various components of the architecture. Configure appropriate security groups and network access control lists (ACLs) to control inbound and outbound traffic.

**Storage Gateway:** Storage Gateway connects on-premises data storage with AWS cloud for seamless data transfer and backup.

**AWS Backup:** AWS Backup simplifies backup and recovery processes by seamlessly protecting on-premises data and storing it securely in the AWS cloud.

**AWS Database Migration Service:** AWS Database Migration Service helps migrate databases to AWS securely and efficiently, minimizing downtime and enabling smooth transitions.

**AWS Certificate Manager:** AWS Certificate Manager provides SSL/TLS certificates to secure websites and applications, ensuring encrypted communication and establishing trust with users.

**AWS Glue Data Catalog:** AWS Glue Data Catalog is a metadata repository that organizes and catalogs data sources, making it easier to discover, manage, and query data for analytics and processing.

**AWS Glue:** AWS Glue is an extract, transform, and load (ETL) service that makes it easy to prepare and transform data for analytics, data warehousing, and machine learning purposes.

**AWS Athena:** AWS Athena allows you to query data stored in Amazon S3 using standard SQL syntax, without the need for traditional database management or infrastructure setup.

![aws-architecture](https://github.com/cheeseig9/AWS-Three-tier-and-Data-Analytics-Architecture/assets/74439890/a13defab-f903-44cc-a0a2-7b50b3732249)
<sup>This architecture might not perfect or ideal :D</sup>
