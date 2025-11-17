## Databases
| Feature | Description |
--------- | -------------
| Concurrency | A real-world application might have multiple users interacting with it simultaneously. A DBMS makes sure that these concurrent interactions succeed without corrupting or losing any data. |
| Consistency | With so many concurrent interactions, the DBMS needs to ensure that the data remains consistent and valid throughout the database. |
| Security    | DBMS provides fine-grained security controls through user authentication and permissions. This will prevent unauthorized viewing or editing of sensitive data. |
| Reliability | It is easy to backup databases and rolls them back to a previous state in case of data loss or a breach. |
| Structured Query Language | SQL simplifies user interaction with the database with an intuitive syntax supporting various operations. |

## Architecture
![](https://cdn.services-k8s.prod.aws.htb.systems/content/modules/33/db_2.png)

## Types of databases
### Relational database

![](https://cdn.services-k8s.prod.aws.htb.systems/content/modules/75/web_apps_relational_db.jpg)

> [!TIP]
> The relationship between tables within a database is called a Schema.

### Non-relational database

- Key-Value
- Document-Based
- Wide-Column
- Graph

![](https://cdn.services-k8s.prod.aws.htb.systems/content/modules/75/web_apps_non-relational_db.jpg)

> [!TIP]
> Non-relational Databases have a different method for injection, known as NoSQL injections. SQL injections are completely different than NoSQL injections. NoSQL injections will be covered in a later module.
