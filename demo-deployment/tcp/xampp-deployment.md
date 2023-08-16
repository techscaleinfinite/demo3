# Xampp deployment

### <mark style="color:blue;">What's Xampp?</mark>

XAMPP is a free and open-source cross-platform web server solution stack, crafted by Apache Friends. It brings together essential components for web development, including the Apache HTTP Server, MariaDB database, and interpreters for PHP and Perl scripting.

**Key Points:**

1. **Comprehensive Solution:** XAMPP packages Apache HTTP Server, MariaDB, PHP, and Perl.
2. **Cross-Platform:** Available for various operating systems, enabling uniform development.
3. **Open Source:** Freely accessible and customizable, promoting collaborative development.
4. **Web Development:** XAMPP provides tools for building dynamic web applications.
5. **Local Server Environment:** Creates a local server on your machine for testing and development.

### <mark style="color:blue;">**Working in Brief:**</mark>



1. **Installation:** Install XAMPP on your computer; it bundles Apache, MariaDB, PHP, and Perl.
2. **Local Web Server:** Launch XAMPP to start a local server environment.
3. **Database Management:** Utilize MariaDB to store and manage your application's data.
4. **Web Development:** Develop and test PHP and Perl scripts on the local server.
5. **Browser Access:** Access your development site through a browser, simulating real deployment.

XAMPP simplifies web development by offering a self-contained environment with essential tools. It empowers developers to create and test web applications seamlessly before deploying them to production servers.

### <mark style="color:blue;">Installation</mark>&#x20;

* &#x20;**Docker image of this application consists of following layers :**

```
'FROM debian:buster' Taking debian:buster as the base image.

And updating and installing all the required softwares like 'openssh-server' 'supervisor' 'net-tools'

Installing the Xampp software. And configuring Xampp to Enable web interface, error display in php.

And creating a /www folder and a symbolic link to it in /opt/lampp/htdocs. This is convenient because it doesn't interfere with xampp, phpmyadmin or other tools in /opt/lampp/htdocs.

And exposing 3306, 22 and 80 ports.
```

#### Deploy Xampp on Scaleinfinite

* &#x20;Go to create apps page and Search scaleinfinite/xampp on the search bar.
* &#x20;Click on install button.
* &#x20;Fill all the reqired feilds.

| PRODUCT NAME |
| ------------ |
| `Xampp`      |

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
* &#x20;Copy the xampp application Hostname without NodePort and search the Url.
* &#x20;You will see the Xampp interface.
* &#x20;Click on PHPMyAdmin button to access the PHPMyAdmin.
* &#x20;Add the /www to the link to access the html application.
* Now you can able to easily access and create application and edit databases in Mysql using Xampp.

### <mark style="color:blue;">Visual SnapShots</mark>



<figure><img src="../../.gitbook/assets/myapps (9).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/xampp (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/phpmyadmin (1) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/index (1).png" alt=""><figcaption></figcaption></figure>

### <mark style="color:blue;">FAQ</mark>

**About Xampp image we used.**

This image is maintained by the scaleinfinite.

**Do the image secure to use ?**

The image is created and verified by the scaleinfinite. it is a 100% secure image.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

#### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
