# Mongo DB

### <mark style="color:blue;">What's Mongo DB?</mark>

MongoDB is a popular open-source, NoSQL database that offers a flexible and scalable way to store and manage data. Here are key points about MongoDB:

1. <mark style="color:orange;">**NoSQL Database**</mark>:
   * MongoDB is a NoSQL database, which means it doesn't use traditional relational structures like tables and rows. Instead, it stores data in flexible and schema-less collections of documents.
2. **Document-Oriented**:
   * Data in MongoDB is stored as JSON-like BSON documents, which are flexible and can hold nested arrays and subdocuments.
3. <mark style="color:orange;">**Scalability**</mark>:
   * MongoDB is designed for horizontal scalability, allowing you to distribute data across multiple servers or clusters to handle larger amounts of data and traffic.
4. **Flexible Schema**:
   * MongoDB's dynamic schema allows you to store different fields in each document, which can be especially useful when dealing with evolving data structures.

### <mark style="color:blue;">**Working in Brief:**</mark>

1. <mark style="color:orange;">**Data Structure**</mark>:
   * MongoDB stores data in collections, which are similar to tables in relational databases. Each collection contains individual documents, analogous to rows in tables.
2. **Document-Oriented Storage**:
   * Data is stored as BSON (Binary JSON) documents, which are flexible and can hold various data types, including strings, numbers, arrays, and subdocuments.
3. <mark style="color:orange;">**Queries and Indexes**</mark>:
   * MongoDB supports a powerful query language for retrieving data. Queries can be used to filter, sort, and aggregate data within a collection.
   * Indexes are used to enhance query performance by creating data structures that facilitate fast data retrieval.
4. **CRUD Operations**:
   * MongoDB supports Create, Read, Update, and Delete (CRUD) operations on documents within collections.
   * Document creation involves inserting a new document into a collection.
   * Reading retrieves documents using queries.
   * Updates modify existing documents.
   * Deletes remove documents from collections

### <mark style="color:blue;">Steps And Procedure</mark>&#x20;

* &#x20;<mark style="background-color:yellow;">**This deployment uses the official  Mongo DB Docker image.**</mark>
* &#x20;Go to create apps page and Search <mark style="color:orange;">Mongo DB</mark> on the search bar.
* &#x20;Click on install button.
* &#x20;Fill all the required fields.
* &#x20;click on Advanced.
* &#x20;Click on the Install button.
* &#x20;You will be redirected to My Apps page, Here you can find all the applications you deployed.
* &#x20;Copy the mongo db application Hostname without NodePort and search the Url.
* &#x20;Now you can create the dashboard and select the data source to visualize the data you need.

### <mark style="color:blue;">Steps to connect with mongo db</mark>

If you want to connect MongoDB Compass to a MongoDB instance running on a different host or IP address, you can follow these steps:

1. <mark style="color:orange;">**Open MongoDB Compass**</mark>: Launch MongoDB Compass on your computer.
2. <mark style="color:orange;">**Click "New Connection"**</mark>: In the MongoDB Compass interface, click on the "New Connection" button to start creating a new connection.
3.  <mark style="color:orange;">**Configure Connection Details**</mark>: In the connection configuration window, follow these steps:

    * **Hostname**: Enter the IP address or hostname of the MongoDB server you want to connect to. In your case, this would be `103.37.96.201`.
    * **Port**: Use the default MongoDB port `27017`.
    * **Authentication**: If the MongoDB server requires authentication, enter the necessary credentials (username and password).

    **Enter Connection URL**: In the connection configuration window, you'll see a single text box labeled "Connection String." Here, you will directly enter the connection URL in the following format:

    ```arduino
     codemongodb://<IP_ADDRESS>:27017
    ```

    Replace `<IP_ADDRESS>` with the actual IP address of the MongoDB server. In your case, the URL would be:

    ```arduino
     codemongodb://103.37.96.201:27017
    ```
4. **Advanced Options** (Optional): If you need to specify additional connection options, you can expand the "Advanced" section. Here, you can configure options like SSL, replica set name, and more.
5. <mark style="color:orange;">**Test Connection**</mark><mark style="color:orange;">:</mark> After entering the connection details, you can click the "Test" button to check if the connection is successful. MongoDB Compass will attempt to connect to the server and validate the settings.
6. <mark style="color:orange;">**Save the Connection**</mark><mark style="color:orange;">:</mark> If the connection test is successful, you can give your connection a name and optionally add it to your favorites. Then click the "Connect" button to establish the connection.
7. <mark style="color:orange;">**Explore and Manage Data**</mark><mark style="color:orange;">:</mark> Once the connection is established, MongoDB Compass will display the databases and collections available on the connected server. You can explore and manage your data using the intuitive graphical interface.

Remember that for the connection to work, the MongoDB server at the specified IP address (`103.37.96.201` in your case) must be reachable from your computer and configured to allow connections from the IP address you are using. Also, if the server requires authentication, make sure to provide the correct credentials during the connection setup.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                  |
| ----------------------------------------------------------------------------------------------------------------------------- |
| [mongo db](https://hub.docker.com/\_/mongo)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                                  |
| --------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: mongo db1(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td>-</td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td><mark style="color:orange;">27017</mark></td></tr></tbody></table>

| Install with Default                                                                                                                                        | Advanced                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">(select this if you want install with default settings if don't have environment value and working directory)</mark> | <mark style="background-color:yellow;">(select this if you want to go with advanced settings, where you select you own environment value and working directory)</mark> |

If you choose Advanced option:

| ENV VARIABLE                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value OR MONGO_INITDB_ROOT_USERNAME=root, MONGO_INITDB_ROOT_PASSWORD=123</code> </p> |

| WORKING DIR                                                                             |
| --------------------------------------------------------------------------------------- |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to MONGO DB Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`Mongo db`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: Mongo1
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `TCP`
   * Port: `27017`
4. <mark style="color:orange;">**Installation Options**</mark>**:**
   * Choose between "Default" or "Advanced" installation.
5. <mark style="color:orange;">**Advanced Installation (Optional**</mark>**):**
   * If selecting "Advanced," you can customize the environment variables and working directory:
   *   **Environment Variables:**

       Environment variables are dynamic values used by a containerized application for configuration. They are defined as key-value pairs, like `API_KEY=xyz`, and provide flexibility to adjust an app's behavior without changing its code.

       * Environment Variables: Define environment variables with keys and values (e.g., `key=value OR MONGO_INITDB_ROOT_USERNAME=root, MONGO_INITDB_ROOT_PASSWORD=123` ).
   *   **Working Directory:**

       The working directory is the starting point inside a container where an app's files are located. It affects relative file paths and operations. For example, if set to `/usr/src/yourAPP`, an app will reference files from there, like `/usr/src/yourAPP/data.txt`.

       * Working Directory: Set the working directory for the application (e.g., `usr/src/yourAPP`).
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an Mongo DB instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-29 122423.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-29 122518.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-29 122706.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:blue;">FAQ</mark>

**About Mongo DB image we used.**

This is the official Mongo DB image.

**Are there any restrictions on adding data sources ?**

you can add any data source that Mongo Db supports.

**Can i deploy older version of  Mondo or my own modified Mongo db image ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
