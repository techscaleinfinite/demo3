---
cover: ../../.gitbook/assets/WordPress-logotype-alternative (1).png
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

# 🖥 WordPress SQLite

### <mark style="color:blue;">What's WordPress SQLite?</mark>

WordPress is a free and open-source content management system written in hypertext preprocessor language and paired with a MySQL or MariaDB database with supported HTTPS. SQLite is an open-source SQL database system that stores data in a text file on a device. It provides a simple and efficient way to manage and retrieve structured information locally.

**Key Points:**

1. <mark style="color:orange;">**Open-Source SQL**</mark>**:** SQLite is freely accessible, offering SQL database capabilities for local storage.
2. **Text File Storage:** Data is stored in a single text file, eliminating the need for a separate server.
3. <mark style="color:orange;">**Lightweight**</mark>**:** SQLite is compact, making it suitable for applications with limited resources.
4. **Embedded Database:** It's integrated within the application, not requiring a separate database server.
5. <mark style="color:orange;">**Self-Contained**</mark>**:** The entire database is contained within a single file, enhancing portability.

### <mark style="color:blue;">**Working in Brief**</mark>**:**

1. **Database Creation:** Applications integrate SQLite by creating a database file.
2. <mark style="color:orange;">**Table Structure**</mark>**:** Define tables with columns to structure the data.
3. **Data Storage:** Insert, update, or delete data within the tables.
4. <mark style="color:orange;">**SQL Queries**</mark>**:** Utilize SQL queries to retrieve specific information from the database.
5. **Local Retrieval:** Applications access data directly from the local SQLite file.

SQLite offers a convenient solution for applications that require structured data storage without the complexity of a traditional database system. Its lightweight nature and self-contained design make it an ideal choice for various applications.

### <mark style="color:blue;">Steps And Procedure</mark>&#x20;

&#x20;<mark style="background-color:yellow;">**Docker image of this application consists of following layers :**</mark>

```
'FROM wordpress:latest' Taking Wordpress as the base image

Used PHP scripts to 'install' the SQLite plugin and setting up the database so that the wordpress will recognize the sqlite database. 

```

#### <mark style="background-color:yellow;">Deploy Wordpress SQLite on Scaleinfinite</mark>

* &#x20;Go to create apps page and Search scaleinfinite/wpsqlite on the search bar.
* &#x20;Click on install button.
* Fill all the required fields.
* &#x20;click on Advanced.
* &#x20;Click on the Install button.
* &#x20;You will be redirected to My Apps page, Here you can find all the applications you deployed.
* &#x20;Copy the wpsqlite application Hostname without NodePort and search the Url.
* Now you can see the wordpress language selection page.
* After selecting language you will be directly redirected to site creation page and fill all the fields like site name and username and so on.
* Then Login with that detials.
* Then you will be redirected to the wordpress Admin dashboard.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                        |
| ----------------------------------------------------------------------------------------------------------------------------------- |
| [`Wpsqlite`](https://hub.docker.com/\_/wordpress)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                                   |
| ---------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: wordpress1(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">80</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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

<mark style="color:purple;">**Step-by-Step Guide to Wordpress SQlite Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`wpsqlite`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `wordpress1`
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `80`
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
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an NGINX instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual SnapShots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 152422 (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 152458 (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 152840.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 152910 (1).png" alt=""><figcaption></figcaption></figure>

</div>



### <mark style="color:blue;">FAQ</mark>

**About Wordpress sqlite image we used.**

This image is maintained by the scaleinfinite.

**Is sqlite good with wordpress ?**

Sqlite is widely used and lightweight database which makes your sight fast.

**Do the image secure to use ?**

The image is created and verified by the scaleinfinite. it is a 100% secure image.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going! &#x20;

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, wordpress

</details>
