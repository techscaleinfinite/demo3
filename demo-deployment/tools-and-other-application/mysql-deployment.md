---
cover: ../../.gitbook/assets/images (1).png
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Mysql deployment

### <mark style="color:blue;">**What's MySQL?**</mark>

**MySQL: Relational Database Management System**

MySQL is a popular open-source Relational Database Management System (RDBMS) that facilitates the organization, storage, and retrieval of structured data efficiently.

**Key Points:**

1. <mark style="color:orange;">**Open-Source RDBMS**</mark>**:** MySQL is freely accessible, providing a robust RDBMS solution.
2. **Structured Data:** It stores data in tables with predefined schemas, ensuring data integrity.
3. <mark style="color:orange;">**SQL Queries**</mark>**:** MySQL uses SQL (Structured Query Language) for data manipulation and retrieval.
4. **Scalability:** It's scalable for small to large-scale applications, supporting high data volumes.
5. <mark style="color:orange;">**Data Integrity**</mark>**:** MySQL enforces data integrity rules, preventing inconsistencies.

### <mark style="color:blue;">**Working in Brief:**</mark>

1. <mark style="color:orange;">**Database Creation**</mark>**:** Set up databases to store related data tables.
2. **Table Definition:** Create tables with predefined column names and data types.
3. **Data Insertion:** Populate tables with data using SQL INSERT statements.
4. <mark style="color:orange;">**Data Retrieval**</mark>**:** Use SQL SELECT queries to retrieve specific data from tables.
5. **Data Manipulation:** Update, delete, or modify data using SQL UPDATE and DELETE statements.

MySQL efficiently manages structured data through its table-based approach, ensuring data accuracy and enabling data-driven applications. Its open-source nature, reliability, and wide community support make it a go-to choice for various web and software projects.

### <mark style="color:blue;">Steps And Procedure</mark>

* **This deployment uses the official MySQL Docker image.**
* Go to create apps page and Search MySQL on the search bar.
* &#x20;Click on install button.
* &#x20;Fill all the required fields.
* &#x20;click on Advanced.
* &#x20;Click on the Install button.
* &#x20;You will be redirected to My Apps page, Here you can find all the applications you deployed.
* &#x20;Copy the mysql application Hostname without NodePort and search the Url.

### <mark style="color:blue;">Installation</mark>&#x20;

| Docker Image                                 |
| -------------------------------------------- |
| 👉[`mysql`](https://hub.docker.com/\_/mysql) |

| Application name                                                               |
| ------------------------------------------------------------------------------ |
| <mark style="background-color:yellow;">Eg: mysql1(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">-</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td><mark style="color:orange;">3306</mark></td></tr></tbody></table>

| Install with Default                                                                                                                                        | Advanced                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">(select this if you want install with default settings if don't have environment value and working directory)</mark> | <mark style="background-color:yellow;">(select this if you want to go with advanced settings, where you select you own environment value and working directory)</mark> |

If you choose Advanced option:

| ENV VARIABLE                                                            |
| ----------------------------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> |

| WORKING DIR                                                                             |
| --------------------------------------------------------------------------------------- |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to Mysql Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`mysql`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `mysql1`
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `TCP`
   * Port: `3306`
4. <mark style="color:orange;">**Installation Options**</mark>**:**
   * Choose between "Default" or "Advanced" installation.
5. <mark style="color:orange;">**Advanced Installation (Optional**</mark>**):**
   * If selecting "Advanced," you can customize the environment variables and working directory:
   *   **Environment Variables:**

       Environment variables are dynamic values used by a containerized application for configuration. They are defined as key-value pairs, like `API_KEY=xyz`, and provide flexibility to adjust an app's behavior without changing its code.

       * Environment Variables: Define environment variables with keys and values (e.g., `key=value`).
   *   **Working Directory:**

       The working directory is the starting point inside a container where an app's files are located. It affects relative file paths and operations. For example, if set to `/usr/src/yourAPP`, an app will reference files from there, like `/usr/src/yourAPP/data.txt`.

       * Working Directory: Set the working directory for the application (e.g., `usr/src/yourAPP`).
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an MYSQL instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshot</mark>

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
