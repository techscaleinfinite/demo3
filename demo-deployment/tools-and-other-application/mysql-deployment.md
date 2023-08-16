# Mysql deployment

#### <mark style="color:blue;">**What's MySQL?**</mark>

**MySQL: Relational Database Management System**

MySQL is a popular open-source Relational Database Management System (RDBMS) that facilitates the organization, storage, and retrieval of structured data efficiently.

**Key Points:**

1. **Open-Source RDBMS:** MySQL is freely accessible, providing a robust RDBMS solution.
2. **Structured Data:** It stores data in tables with predefined schemas, ensuring data integrity.
3. **SQL Queries:** MySQL uses SQL (Structured Query Language) for data manipulation and retrieval.
4. **Scalability:** It's scalable for small to large-scale applications, supporting high data volumes.
5. **Data Integrity:** MySQL enforces data integrity rules, preventing inconsistencies.

#### <mark style="color:blue;">**Working in Brief:**</mark>

1. **Database Creation:** Set up databases to store related data tables.
2. **Table Definition:** Create tables with predefined column names and data types.
3. **Data Insertion:** Populate tables with data using SQL INSERT statements.
4. **Data Retrieval:** Use SQL SELECT queries to retrieve specific data from tables.
5. **Data Manipulation:** Update, delete, or modify data using SQL UPDATE and DELETE statements.

MySQL efficiently manages structured data through its table-based approach, ensuring data accuracy and enabling data-driven applications. Its open-source nature, reliability, and wide community support make it a go-to choice for various web and software projects.

#### <mark style="color:blue;">Installation</mark>

* **This deployment uses the official Mysql Docker image.**
* Go to create apps page and Search mysql on the search bar.
* &#x20;Click on install button.
* &#x20;Fill all the reqired feilds.

| PRODUCT NAME |
| ------------ |
| `mysql`      |

`PROTOCOL`

| HTTP | TCP/UDP |
| ---- | ------- |
| `80` |         |

* &#x20;click on Advanced.

| ENV VARIABLE        | WHITELIST                                       | WORKING DIR                   |
| ------------------- | ----------------------------------------------- | ----------------------------- |
| `Give env variable` | `If you want to white list any ports list here` | `WORKDIR for the application` |

* &#x20;Click on the Install button.
* &#x20;You will be redirected to My Apps page, Here you can find all the applications you deployed.
* &#x20;Copy the mysql application Hostname without NodePort and search the Url.

#### <mark style="color:blue;">Visual Snapshot</mark>

<figure><img src="../../.gitbook/assets/my.png" alt=""><figcaption></figcaption></figure>



### <mark style="color:blue;">FAQ</mark>

**About mysql image we used.**

This is the official mysql image.

**Are there any restrictions on adding data sources ?**

you can add any data source that mysql supports.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

#### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
