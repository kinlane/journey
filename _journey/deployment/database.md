---
class:
- line
rel:
- self
properties:
  name: Database
  sort: 1017
  level: 2
  description: The backend database schema, infrastructure, and other relevant information
    regarding how data is managed, and leveraged to deploy APIs, and deliver the resources
    needed to make the services work.
  service:
    - name: SlashDB
      description: SlashDB connects your internal databases and constructs a REST/HTTP web service, easily making database content accessible by URLs for getting, updating, inserting and deleting in a secure way.  SlashDB provides connectors for Microsoft SQL Server, Oracle, MySQL, PostGreSQL, IBM DB2 and Sybase--covering the top 5 databases you will find in the enterprise or small to medium businesses. SlashDB automatically turns databases into online resource so their content becomes accessible to authorized web, mobile and enterprise applications for reading and writing under standard data formats. Technically speaking, it makes REST APIs out of relational databases.
      url: http://www.slashdb.com/
    - name: Azure SQL Database
      description: Azure SQL Database is the intelligent, fully managed relational cloud database service that provides the broadest SQL Server engine compatibility, so you can migrate your SQL Server databases without changing your apps. Accelerate app development and make maintenance easy and productive using the SQL tools you love to use. Take advantage of built-in intelligence that learns app patterns and adapts to maximize performance, reliability, and data protection.
      url: https://azure.microsoft.com/en-us/services/sql-database/
    - name: Amazon Relational Database Service (RDS) – AWS
      description: Amazon Relational Database Service (Amazon RDS) makes it easy to set up, operate, and scale a relational database in the cloud. It provides cost-efficient and resizable capacity while automating time-consuming administration tasks such as hardware provisioning, database setup, patching and backups.
      url: https://aws.amazon.com/rds/
    - name: Google Cloud Spanner
      description: Cloud Spanner is the first and only relational database service that is both strongly consistent and horizontally scalable. With Cloud Spanner you enjoy all the traditional benefits of a relational database ACID transactions, relational schemas (and schema changes without downtime), SQL queries, high performance, and high availability. But unlike any other relational database service, Cloud Spanner scales horizontally, to hundreds or thousands of servers, so it can handle the highest of transactional workloads. With automatic scaling, synchronous data replication, and node redundancy, Cloud Spanner delivers up to 99.999% of availability for your mission critical applications. In fact, Google’s internal Spanner service has been handling millions of queries per second from many Google services for years.
      url: https://cloud.google.com/spanner/                        
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Database
  links:
  - rel:
    - self
    href: deployment/database/
  - rel:
    - parent
    href: deployment/
links:
- rel:
  - self
  href: deployment/database/
- rel:
  - parent
  href: deployment/
...
