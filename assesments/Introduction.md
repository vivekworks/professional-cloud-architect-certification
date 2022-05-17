## Introduction

1. Building for Builders LLC manufactures equipment used in residential and commercial building. Each of its 500,000 pieces of equipment in use around the globe has IoT devices collecting data about the state of equipment. The IoT data is streamed from each device every 10 seconds. On average, 10 KB of data is sent in each message. The data will be used for predictive maintenance and product development. The company would like to use a managed service in Google Cloud. What would you recommend?

    - Apache Cassandra
    - Cloud Bigtable
    - BigQuery
    - Cloud SQL

    <details>
        <summary>Click for Correct Answer</summary>
        Option B is correct. Bigtable is the best option for streaming IoT data, since it supports low-latency writes and is designed to scale to support petabytes of data. Option A is incorrect because Apache Cassandra is not a managed database in GCP. Option C is incorrect because BigQuery is a data warehouse. While it is a good option for analyzing large volumes of data, Bigtable is a better option for ingesting the data. Option D is incorrect. CloudSQL is a managed relational database. The use case does not require a relational database, and Bigtable's scalability is a better fit with the requirements.
    </details>

2. You have developed a web application that is becoming widely used. The front end runs in Google App Engine and scales automatically. The backend runs on Compute Engine in a managed instance group. You have set the maximum number of instances in the backend managed instance group to five. You do not want to increase the maximum size of the managed instance group or change the VM instance type, but there are times the front end sends more data than the backend can keep up with and data is lost. What can you do to prevent the loss of data?

- Use an unmanaged instance group.
- Store ingested data in Cloud Storage.
- Have the front end write data to a Cloud Pub/Sub topic, and have the backend read from that topic.
- Store ingested data in BigQuery.

    <details>
        <summary>Click for Correct Answer</summary>
        The correct answer is C. A Cloud Pub/Sub topic would decouple the front end and backend, provide a managed and scalable message queue, and store ingested data until the backend can process it. Option A is incorrect. Switching to an unmanaged instance group will mean that the instance group cannot autoscale. Option B is incorrect. You could store ingested data in Cloud Storage, but it would not be as performant as the Cloud Pub/Sub solution. Option D is incorrect because BigQuery is a data warehouse and not designed for this use case.
    </details>

You are setting up a cloud project and want to assign members of your team different roles that have appropriate permissions for their responsibilities. What GCP service would you use to do that?

- Cloud Identity
- Identity and Access Management (IAM)
- Cloud Authorizations
- LDAP

    <details>
        <summary>Click for Correct Answer</summary>
        The correct answer is B. IAM is used to manage roles and permissions. Option A is incorrect. Cloud Identity is a service for creating and managing identities. Option C is incorrect. There is no GCP service with that name at this time. Option D is incorrect. LDAP is not a GCP service.
    </details>

You would like to run a custom stateless container in a managed Google Cloud service. What are your three options?

- App Engine Standard, Cloud Run, and Kubernetes Engine
- App Engine Flexible, Cloud Run, and Kubernetes Engine
- Compute Engine, Cloud Functions, and Kubernetes Engine
- Cloud Functions, Cloud Run, and App Engine Flexible

    <details>
        <summary>Click for Correct Answer</summary>
        The correct answer is B. You can run custom stateless containers in App Engine Flexible, Cloud Run, and Kubernetes Engine. Option A is incorrect because App Engine Standard does not support custom containers. Option C is incorrect because Compute Engine is not a managed service and Cloud Functions does not support custom containers. Option D is incorrect because Cloud Functions does not support custom containers.
    </details>

PhotosForYouToday prints photographs and ships them to customers. The front-end application uploads photos to Cloud Storage. Currently, the back end runs a cron job that checks Cloud Storage buckets every 10 minutes for new photos. The product manager would like to process the photos as soon as they are uploaded. What would you use to cause processing to start when a photo file is saved to Cloud Storage?
A Cloud Function
An App Engine Flexible application
A Kubernetes pod
A cron job that checks the bucket more frequently

The chief financial officer of your company believes that you are spending too much money to run an on-premises data warehouse and wants to migrate to a managed cloud solution. What GCP service would you recommend for implementing a new data warehouse in GCP?
Compute Engine
BigQuery
Cloud Dataproc
Cloud Bigtable

A government regulation requires you to keep certain financial data for seven years. You are not likely to ever retrieve the data, and you are only keeping it to comply with regulations. There are approximately 500 TB of financial data for each year that you are required to save. What is the most cost-effective way to store this data?
Cloud Storage multiregional storage
Cloud Storage Nearline storage
Cloud Storage Archive storage
Cloud Storage persistent disk storage

Global Games Enterprises Inc. is expanding from North America to Europe. Some of the games offered by the company collect personal information. With what additional regulation will the company need to comply when it expands into the European market?
HIPAA
PCI-DSS
GDPR
SOX

Your team is developing a Tier 1 application for your company. The application will depend on a PostgreSQL database. Team members do not have much experience with PostgreSQL and want to implement the database in a way that minimizes their administrative responsibilities for the database. What managed service would you recommend?
Cloud SQL
Cloud Dataproc
Cloud Bigtable
Cloud PostgreSQL

What is a service-level indicator?
A metric collected to indicate how well a service-level objective is being met
A type of log
A type of notification sent to a sysadmin when an alert is triggered
A visualization displayed when a VM instance is down

Developers at MakeYouFashionable have adopted agile development methodologies. Which tool might they use to support CI/CD?
Google Docs
Jenkins
Apache Cassandra
Clojure

You have a backlog of audio files that need to be processed using a custom application. The files are stored in Cloud Storage. If the files were processed continuously on three n2-standard-4 instances, the job could complete in two days. You have 30 days to deliver the processed files, after which they will be sent to a client and deleted from your systems. You would like to minimize the cost of processing. What might you do to help keep costs down?
Store the files in Coldline storage.
Store the processed files in multiregional storage.
Store the processed files in Cloud CDN.
Use preemptible VMs.

You have joined a startup selling supplies to visual artists. One element of the company's strategy is to foster a social network of artists and art buyers. The company will provide e-commerce services for artists and earn revenue by charging a fee for each transaction. You have been asked to collect more detailed business requirements. What might you expect as an additional business requirement?
The ability to ingest streaming data
A recommendation system to match buyers to artists
Compliance with SOX regulations
Natural language processing of large volumes of text

You work for a manufacturer of specialty die cast parts for the aerospace industry. The company has built a reputation as the leader in high-quality, specialty die cast parts, but recently the number of parts returned for poor quality is increasing. Detailed data about the manufacturing process is collected throughout every stage of manufacturing. To date, the data has been collected and stored but not analyzed. There is a total of 20 TB of data. The company has a team of analysts familiar with spreadsheets and SQL. What service might you recommend for conducting preliminary analysis of the data?
Compute Engine
Kubernetes Engine
BigQuery
Cloud Functions

A client of yours wants to run an application in a highly secure environment. They want to use instances that will only run boot components verified by digital signatures. What would you recommend they use in Google Cloud?
Preemptible VMs
Managed instance groups
Cloud Functions
Shielded VMs

You have installed the Google Cloud SDK. You would now like to work on transferring files to Cloud Storage. What command-line utility would you use?
bq
gsutil
cbt
gcloud

Kubernetes pods sometimes need access to persistent storage. Pods are ephemeral—they may shut down for reasons not in control of the application running in the pod. What mechanism does Kubernetes use to decouple pods from persistent storage?
PersistentVolumes
Deployments
ReplicaSets
Ingress

An application that you support has been missing service-level objectives, especially around database query response times. You have reviewed monitoring data and determined that a large number of database read operations is putting unexpected load on the system. The database uses PostgreSQL, and it is running in Compute Engine. You have tuned SQL queries, and the performance is still not meeting objectives. Of the following options, which would you try next?
Migrate to a NoSQL database.
Move the database to Cloud SQL.
Use read replicas.
Move some of the data out of the database to Cloud Storage.

You are running a complicated stream processing operation using Apache Beam. You want to start using a managed service. What GCP service would you use?
Cloud Dataprep
Cloud Dataproc
Cloud Dataflow
Cloud Identity

Your team has had several incidents in which Tier 1 and Tier 2 services were down for more than one hour. After conducting a few retrospective analyses of the incidents, you have determined that you could identify the causes of incidents faster if you had a centralized log repository. What GCP service could you use for this?
Cloud Logging
Cloud Monitoring
Cloud SQL
Cloud Trace

A Global 2000 company has hired you as a consultant to help architect a new logistics system. The system will track the location of parts as they are shipped between company facilities in Europe, Africa, South America, and Australia. Anytime a user queries the database, they must receive accurate and up-to-date information; specifically, the database must support strong consistency. Users from any facility may query the database using SQL. What GCP service would you recommend?
Cloud SQL
BigQuery
Cloud Spanner
Cloud Dataflow

A database architect for a game developer has determined that a NoSQL document database is the best option for storing players’ possessions. What GCP service would you recommend?
Cloud Firestore
Cloud Storage
Cloud Dataproc
Cloud Bigtable

A major news agency is seeing increasing readership across the globe. The CTO is concerned that long page-load times will decrease readership. What might the news agency try to reduce the page-load time of readers around the globe?
Regional Cloud Storage
Cloud CDN
Fewer firewall rules
Virtual private network

What networking mechanism allows different VPC networks to communicate using private IP address space, as defined in RFC 1918?
ReplicaSets
Custom subnets
VPC network peering
Firewall rules

You have been tasked with setting up disaster recovery infrastructure in the cloud that will be used if the on-premises data center is not available. What network topology would you use for a disaster recovery environment?
Meshed topology
Mirrored topology
Gated egress topology
Gated ingress topology