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

# WordPress SQLite

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

| Docker Image                                      |
| ------------------------------------------------- |
| [`Wpsqlite`](https://hub.docker.com/\_/wordpress) |

`PROTOCOL`

| HTTP | TCP/UDP |
| ---- | ------- |
| `80` |         |

| ENV VARIABLE                                                            | WHITELIST                                       | WORKING DIR                                       |
| ----------------------------------------------------------------------- | ----------------------------------------------- | ------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> | `If you want to white list any ports list here` | `WORKDIR for the application. Eg:usr/src/yourAPP` |

### <mark style="color:blue;">Visual SnapShots</mark>

<div>

<figure><img src="../../.gitbook/assets/wordpress-dashboard (1).jpg" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/wordpress-login (2).jpg" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/wordpress-welcome (2).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/wordpress-lang (2).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/myapps (8).png" alt=""><figcaption></figcaption></figure>

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
