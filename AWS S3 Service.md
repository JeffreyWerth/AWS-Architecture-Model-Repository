
#### AWS S3 Service [Model Description and Dictionary]

Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. Customers of all sizes and industries can use Amazon S3 to store and protect any amount of data for a range of use cases, such as data lakes, websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon S3 provides management features so that you can optimize, organize, and configure access to your data to meet your specific business, organizational, and compliance requirements.

| Name                    | Description                                                                                               | Model Element |
| ----------------------- | --------------------------------------------------------------------------------------------------------- | ------------- |
| S3 Standard             | Storage class that offers high durability, availability, and performance.                                 | Block         |
| S3 Intelligent Tiering  | Storage class that delivers automatic storage cost savings.                                               | Block         |
| S3 Standard Infrequent  | Storage class that is access less frequently but requires rapid access.                                | Block         |
| S3 1 Zone Intelligent   | Storage class in one zone that delivers automatic storage cost savings.                                   | Block         |
| S3 Glacier              | Storage class that delivers the lowest-cost for long-lived data that is rarely accessed.                  | Block         |
| S3 Glacier Deep Archive | Storage class with lowest-cost and long-term retention and digital preservation of data.                  | Block         |
| s3standard.namespace    | Is the bucket URL address where objects are store within a region.                                       | Block         |
| networkEndpoint         | S3 access points to buckets with dedicated access policies.                                               | Full Port     |
| verifyIAM               | Operation to verify Identity and Access Management for user or group to a AWS service.                    | Operation     |
| rwPermission            | Operation to grant read and write permissions for individual buckets/objects to authorized user or group. | Operation     |
| S3objectOWnership       | Signal to disable Access Control Lists and take ownership of every object in a bucket.                    | Reception     |
| S3objectEncryption      | Signal to turn on data encryption for data on transit SSL/TLS or client-side encryption in S3 bucket.     | Reception     |
| accessAnalyserforS3     |                                                                                                           | Operation     |
| S3objectLambda          |                                                                                                           |               |
| eventNotifications      |                                                                                                           |               |
|                         |                                                                                                           |               |

#### AWS S3 Service [Structure Diagrams]

##### AWS S3 Service Bucket bdd

![AWS S3 Service Bucket](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/Packages/S3/AWS%20S3%20Service-S3%20Bucket%20bdd.svg)

##### S3 Service Storage Classes bdd

![AWS S3 Service Storage Classes](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/Packages/S3/AWS%20S3%20Service-S3%20Storage%20Classes%20bdd.svg)

#### S3 Service [Behavioral Diagrams]

##### S3 Service Lifecycle Classes stm

![AWS S3 Service Lifecycle](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/Packages/S3/AWS%20S3%20Service-S3%20Lifecycle%20stm.svg)

#### S3 Service [Requirements Diagrams]
