---
description: >-
  Your trusted database browser. Simplify MySQL and MariaDB management through a
  user-friendly web interface, making data organization and access a breeze.
cover: ../../.gitbook/assets/XEMoGak7.png
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

# 🖥 PHPmyADMIN Deployment

### <mark style="color:blue;">What's  php myadmin?</mark>

<mark style="color:orange;">phpMyAdmin is like a trusted browser for your MySQL and MariaDB databases, simplifying the often complex world of database management.</mark> Here's how it all goes:

**Web display :** phpMyAdmin resides directly in your web browser. To get started, all you need to do is visit the phpMyAdmin URL hosted on your web server. It's like opening a book in your library, only your library is digital.

**Database connection:** Before you begin, you need to establish a connection to your MySQL or MariaDB database server. Think of it as a secret connection: your hostname or IP address, your username, and the associated password. If necessary, you can also specify the port number.

**User authentication:** Once you've knocked on the virtual door of the database, phpMyAdmin will usually ask you to prove that you are who you say you are. You enter your username and password, then phpMyAdmin will check the database server user account.

**Database selection:** After passing the virtual browser, it's time to choose the database you want to work with. phpMyAdmin gives you a list of all the databases available on the server. You can select an existing playground or create a completely new one for your data.

**Navigating the database:** In the database of your choice, phpMyAdmin will become your tour guide. It presents the database structure in a user-friendly interface, often organized in neat tabs and an extensible tree structure. It's like having a map that guides you through the intricacies of the database. Array management: Once inside, you can put on your manager's hat. phpMyAdmin allows you to create new tables, modify existing ones, or even start them up if no longer needed. You can also view a table diagram, including columns, data types, and indexes. It's like being the architect of your data world.

Basically, phpMyAdmin is your trusted companion that makes browsing through your database smoother and easier to access, even for seasoned non-techies. experience. It's like having a trained librarian in your digital library, helping you organize and understand the treasures in your database. 📚🔍📊

### <mark style="color:blue;">**How It Works:**</mark>

<mark style="color:orange;">phpMyAdmin works as a web-based interface for managing MySQL and MariaDB databases. Here's a step-by-step overview of how it operates:</mark>

1. **Accessing the Interface**: Users access phpMyAdmin by navigating to its URL through a web browser. The phpMyAdmin interface is hosted on a web server, often the same server where the MySQL or MariaDB database is running.
2. **Login and Authentication**: Upon reaching the phpMyAdmin login page, users are required to provide valid login credentials, including a username and password. These credentials are checked against the user accounts configured in the MySQL or MariaDB database server.
3. **Selecting a Database**: After successful authentication, users can choose a specific database to work with. phpMyAdmin lists all available databases on the server. Users can either select an existing database or create a new one.
4. **Navigation and Database Structure**: Once a database is selected, phpMyAdmin provides a user-friendly interface for navigating its structure. This typically includes a sidebar with an expandable tree view of tables, views, and other database objects. Users can click on these objects to view their details.
5. **Table Management**: Users can manage database tables by creating new tables, modifying existing ones, or deleting tables. phpMyAdmin offers forms for defining table structures, including columns, data types, and indexes.
6. **Data Manipulation**: phpMyAdmin allows users to insert, update, and delete data within database tables. It offers a user-friendly form-based interface for data manipulation.
7. **SQL Query Execution**: For advanced users, phpMyAdmin provides an SQL query interface. Users can execute custom SQL queries directly against the database. This is useful for complex operations, custom reports, and data retrieval.

### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official phpmyadmin Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the <mark style="color:orange;">phpmyadmin</mark> application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the phpmyadmin application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the phpmyadmin webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed the phpmyadmin application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                           |
| -------------------------------------------------------------------------------------------------------------------------------------- |
| [`phpmyadmin`](https://hub.docker.com/\_/phpmyadmin)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                             |
| ---------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: php1(you can put any name)</mark> |

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

| WORKING DIR                                                                                 |
| ------------------------------------------------------------------------------------------- |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p>     |
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                     |
| -v /some/local/directory/config.user.inc.php:/etc/phpmyadmin/config.user.inc.php phpmyadmin |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to phpmyadmin Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`phpmyadmin`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `php1`
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
       * \-v /some/local/directory/config.user.inc.php:/etc/phpmyadmin/config.user.inc.php phpmyadmin
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an phpmyadmin instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-01 154231.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-01 154259.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About** phpmyadmin **image we used.**

This is the official phpmyadmin image.

**Can I deploy my own** phpmyadmin **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, database, php

</details>
