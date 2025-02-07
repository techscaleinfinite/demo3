---
description: >-
  Your open-source data librarian. Organize, store, and retrieve structured
  information seamlessly with SQL fluency and scalability, all without breaking
  the bank.
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

# 🖥 Mysql deployment

### <mark style="color:blue;">**What's MySQL?**</mark>

<mark style="color:orange;">MySQL is like a trusted librarian for your data, helping you organize, store, and retrieve structured information with ease. Here are the key points that make MySQL stand out:</mark>

**Open-Source RDBMS:** MySQL is a generous soul—it's open-source and free to use. You get a robust and reliable Relational Database Management System (RDBMS) without breaking the bank.

**Structured Data:** Think of MySQL as your data's personal organizer. It neatly arranges your information into tables with predefined schemas, ensuring that your data stays organized and behaves itself.

**SQL Queries:** MySQL is fluent in the language of data—SQL (Structured Query Language). It's like having a skilled translator that understands your every request, making data manipulation and retrieval a breeze.

**Scalability:** Whether you're building a cozy blog or a massive e-commerce empire, MySQL can scale with you. It's like having a magic storage cabinet that can accommodate everything from a few trinkets to a treasure trove of data.

**Data Integrity:** MySQL is your guardian of data integrity. It's like a diligent security guard, enforcing rules to prevent data inconsistencies and maintaining the sanctity of your information.

In a world where data is king, MySQL reigns supreme as the go-to solution for managing structured data. It's like having a trusty librarian who not only knows where every book is but also ensures they're all in perfect order. So, whether you're building a simple app or a complex system, MySQL is your steadfast partner in data management

### <mark style="color:blue;">**Working in Brief:**</mark>

<mark style="color:orange;">**Database Creation:**</mark> MySQL makes setting up your data playground a breeze. You can create databases to neatly organize related data tables. It's like building different rooms in your data house, each with its own purpose.

**Table Definition:** Inside these databases, MySQL lets you define tables with specific column names and data types. Think of it as designing the blueprint for your data structure—a place for each piece of information.

**Data Insertion:** Once you've set the stage, you can start populating your tables with data using SQL INSERT statements. It's like adding books to your library shelves, one by one, ensuring your data is neatly organized.

**Data Retrieval:** Need to find something specific? MySQL's got you covered with SQL SELECT queries. It's like having a skilled detective that can find that one clue you need in a sea of information.

<mark style="color:orange;">**Data Manipulation:**</mark> And when things change or need a tweak, MySQL is your tool of choice. You can use SQL UPDATE and DELETE statements to modify, update, or remove data. It's like having a data workshop where you can craft and refine your information.

MySQL's approach to data management is all about precision and reliability. It's like having a master craftsman overseeing your data, making sure it's accurate, accessible, and ready to power your data-driven applications. Its open-source nature, rock-solid reliability, and the support of a vast community make it a top pick for a wide range of web and software projects.

### <mark style="color:blue;">Steps And Procedure</mark>

*

    <mark style="background-color:purple;">**This deployment utilizes the official MySql  image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the <mark style="color:orange;">mysql</mark> application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the <mark style="color:orange;">mysql</mark>  application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the  <mark style="color:orange;">mysql</mark> webpage and explore its content.

### <mark style="color:blue;">Installation</mark>&#x20;

| Docker Image                                                                                                                 |
| ---------------------------------------------------------------------------------------------------------------------------- |
| [`mysql`](https://hub.docker.com/\_/mysql)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

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

| WORKING DIR                                                                                                   |
| ------------------------------------------------------------------------------------------------------------- |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p>                       |
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                                       |
| <p></p><pre class="language-console"><code class="lang-console">-v /my/custom:/etc/mysql/conf.d
</code></pre> |

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
       * <mark style="color:red;">Here use ( use the path after   " :"  )</mark>
       *

           ```console
           -v /my/custom:/etc/mysql/conf.d
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.



By following these steps, you can effortlessly deploy an MYSQL instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

<mark style="color:orange;">**Connecting to MySQL Database via MySQL Client**</mark>

When deploying a MySQL application, you can't directly connect to it via a web browser as you would with HTTP applications. Instead, you need to use a MySQL client to establish a connection using the application's IP address, username, and password. Here's how to do it:

1. **Install MySQL Client:** If you don't have MySQL client installed, you can download and install it on your local machine from the official MySQL website.
2. **Gather Connection Details:** After deploying your MySQL application, note down its IP address, username, and password. You might have received these details during the deployment process or through an email.
3. **Open MySQL Client:** Open your MySQL client application on your local machine.
4. **Create a New Connection:** Look for an option to create a new connection or establish a new session. This might vary based on the MySQL client you are using.
5. **Enter Connection Details:** In the connection setup, provide the following details:
   * Host: The IP address of your deployed MySQL application.
   * Username: The MySQL username associated with your application.
   * Password: The corresponding password for the provided username.
6. **Connect:** Once you've entered the details, click on the "Connect" or "Log In" button to establish a connection.
7. **Execute Queries:** After successfully connecting, you'll be able to execute SQL queries, manage databases, and perform various database-related operations using the MySQL client interface.

### <mark style="color:blue;">Visual Snapshot</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-23 160349 (2).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/ccvc.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/vbvb.png" alt=""><figcaption></figcaption></figure>

</div>

<div>

<figure><img src="../../.gitbook/assets/bbn.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/mhjyjy.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-23 161329 (3).png" alt=""><figcaption></figcaption></figure>

</div>

<div>

<figure><img src="../../.gitbook/assets/bbf.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/jjj.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



{% embed url="https://youtu.be/dr-P1VnJo-Q" %}

### <mark style="color:blue;">FAQ</mark>

**About mysql image we used.**

This is the official mysql image.

**Are there any restrictions on adding data sources ?**

you can add any data source that mysql supports.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

#### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, database, mysql

</details>
