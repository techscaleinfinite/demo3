---
cover: ../../.gitbook/assets/WordPress-logotype-alternative.png
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

# WordPress MySQL

### <mark style="color:blue;">What's WordPress?</mark>

WordPress is a dynamic, open-source content management system, coded in hypertext preprocessor (PHP), seamlessly paired with a MySQL or MariaDB database, and fortified with HTTPS support. It's your platform for creating and managing websites with ease.

**Key Points:**

1. <mark style="color:orange;">**Open-Source CMS**</mark>**:** WordPress is freely accessible, offering a flexible foundation for website creation.
2. **PHP-Powered:** The core of WordPress is written in PHP, a versatile scripting language.
3. <mark style="color:orange;">**Database Pairing**</mark>**:** WordPress relies on MySQL or MariaDB databases to store content, settings, and more.
4. **HTTPS Supported:** Security is prioritized with built-in HTTPS support, encrypting data transmission.

### <mark style="color:blue;">**Working in Brief**</mark>

1. <mark style="color:orange;">**Content Creation**</mark>**:** Craft and publish web content through an intuitive dashboard.
2. **Database Interaction:** WordPress communicates with the MySQL/MariaDB database to store and retrieve content, settings, and user data.
3. <mark style="color:orange;">**Themes & Plugins**</mark>**:** Enhance functionality and design using themes for appearance and plugins for added features.
4. **Dynamic Pages:** PHP processes user requests, dynamically generating web pages and assembling content.
5. <mark style="color:orange;">**HTTPS Encryption**</mark>**:** Data transmitted between users and the website is encrypted, enhancing security.

WordPress simplifies website management, offering a user-friendly interface for content creation and a robust ecosystem of themes and plugins to customize your site's look and features.

### <mark style="color:blue;">Steps And Procedure</mark>

&#x20;**Docker image of this application consists of following layers :**

```
'FROM ubuntu:14.04' Taking ubuntu:14.04 as the base image.

And updating and installing all the required softwares like 'mysql-server' 'mysql-client' 'nginx' for better performance 'php5-fpm' 'php5-mysql'.

And installing all the required softwares for Wordpress 'php5-curl' 'php5-gd' 'php5-intl'

Done configurations in required files like adding nginx keepalive_timeout and wordpress upload and post max file size.

Exposing 3306 and 80 ports on the container. 
```

#### Deploy Wordpress Mysql on Scaleinfinite

* &#x20;Go to create apps page and Search scaleinfinite/wpmysql on the search bar.
* &#x20;Click on install button.
* Fill all the reqired fields.
* &#x20;click on Advanced.
* &#x20;Click on the Install button.
* You will be redirected to My Apps page, Here you can find all the applications you deployed.
* Copy the wpmysql application Hostname without NodePort and search the Url.
* Now you can see the wordpress language selection page.
* After selecting language you will be directly redirected to site creation page and fill all the fields like site name and username and so on.
* Then Login with that detials.
* Then you will be redirected to the WordPress Admin dashboard.

### <mark style="color:blue;">Installation</mark>&#x20;

| Docker Image                                     |
| ------------------------------------------------ |
| [`Wpmysql`](https://hub.docker.com/\_/wordpress) |

`PROTOCOL`

| HTTP | TCP/UDP |
| ---- | ------- |
| `80` |         |

| ENV VARIABLE                                                            | WHITELIST                                       | WORKING DIR                                       |
| ----------------------------------------------------------------------- | ----------------------------------------------- | ------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> | `If you want to white list any ports list here` | `WORKDIR for the application. Eg:usr/src/yourAPP` |

### <mark style="color:blue;">Visual snapshots</mark>

<figure><img src="../../.gitbook/assets/myapps (5).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/wordpress-lang (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/wordpress-welcome (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/wordpress-login (1).jpg" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-12 153350.png" alt=""><figcaption></figcaption></figure>

### <mark style="color:purple;">FAQ</mark>

**About Wordpress mysql image we used.**

This image is maintained by the scaleinfinite.

**Is Mysql is in the same container ?**

Yes, both WordPress and MySQL are inbuilt into the same container securely.

**Do the image secure to use ?**

The image is created and verified by the scaleinfinite. it is a 100% secure image.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
