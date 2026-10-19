
| AWS Resource | Use This When… | Why / Example |
|---|---|---|
| **S3 — Object storage** | You need to store files such as images, videos, backups, logs, or datasets. | Stores objects in buckets without managing a server. **Example:** property listing photos. |
| **EBS — Block storage** | Your EC2 instance needs a disk for its operating system, applications, or data. | Acts like an attached hard drive with fast reads and writes. **Example:** the boot disk for your Flask server. |
| **EFS — Shared file storage** | Multiple Linux servers need to access the same files and folders. | Provides a shared filesystem that grows as you add files. **Example:** several web servers accessing shared uploads. |
| **RDS — Relational database (SQL)** | You need structured tables, relationships, SQL queries, and joins. | Manages common database administration tasks. **Example:** linked tables for users, properties, and reservations. |
| **DynamoDB — NoSQL database** | You need fast key-based lookups at large scale, with predictable access patterns. | Provides a managed, serverless key-value/document database. **Example:** retrieving a shopping cart by user ID. |
