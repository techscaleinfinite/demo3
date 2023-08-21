---
cover: ../../.gitbook/assets/images (2).png
coverY: 0
layout:
  cover:
    visible: true
    size: full
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

# Xampp deployment

### <mark style="color:blue;">What's Xampp?</mark>

XAMPP is a free and open-source cross-platform web server solution stack, crafted by Apache Friends. It brings together essential components for web development, including the Apache HTTP Server, MariaDB database, and interpreters for PHP and Perl scripting.

**Key Points:**

1. <mark style="color:orange;">**Comprehensive Solution**</mark>**:** XAMPP packages Apache HTTP Server, MariaDB, PHP, and Perl.
2. **Cross-Platform:** Available for various operating systems, enabling uniform development.
3. <mark style="color:orange;">**Open Source**</mark>**:** Freely accessible and customizable, promoting collaborative development.
4. **Web Development:** XAMPP provides tools for building dynamic web applications.
5. <mark style="color:orange;">**Local Server Environment**</mark>**:** Creates a local server on your machine for testing and development.

### <mark style="color:blue;">**Working in Brief:**</mark>



1. **Installation:** Install XAMPP on your computer; it bundles Apache, MariaDB, PHP, and Perl.
2. <mark style="color:orange;">**Local Web Server**</mark>**:** Launch XAMPP to start a local server environment.
3. **Database Management:** Utilize MariaDB to store and manage your application's data.
4. <mark style="color:orange;">**Web Development**</mark>**:** Develop and test PHP and Perl scripts on the local server.
5. **Browser Access:** Access your development site through a browser, simulating real deployment.

XAMPP simplifies web development by offering a self-contained environment with essential tools. It empowers developers to create and test web applications seamlessly before deploying them to production servers.

### &#x20;<mark style="color:blue;">Steps And Procedure</mark>

* &#x20;**Docker image of this application consists of following layers :**

```
'FROM debian:buster' Taking debian:buster as the base image.

And updating and installing all the required softwares like 'openssh-server' 'supervisor' 'net-tools'

Installing the Xampp software. And configuring Xampp to Enable web interface, error display in php.

And creating a /www folder and a symbolic link to it in /opt/lampp/htdocs. This is convenient because it doesn't interfere with xampp, phpmyadmin or other tools in /opt/lampp/htdocs.

And exposing 3306, 22 and 80 ports.
```

#### Deploy Xampp on Scaleinfinite

* &#x20;Go to create apps page and Search <mark style="color:orange;">scaleinfinite/xampp</mark> on the search bar.
* &#x20;Click on install button.
* &#x20;Fill all the required fields.
* &#x20;click on Advanced.
* &#x20;Click on the Install button.
* &#x20;You will be redirected to My Apps page, Here you can find all the applications you deployed.
* &#x20;Copy the xampp application Hostname without NodePort and search the Url.
* &#x20;You will see the Xampp interface.
* &#x20;Click on PHPMyAdmin button to access the PHPMyAdmin.
* &#x20;Add the /www to the link to access the html application.
* Now you can able to easily access and create application and edit databases in Mysql using Xampp.

### <mark style="color:blue;">Installation</mark>&#x20;

| Docker Image                                                                                                  |
| ------------------------------------------------------------------------------------------------------------- |
| [`Xampp`](https://hub.docker.com/r/tomsik68/xampp/)<mark style="background-color:yellow;">👈(click me)</mark> |

| Application name                                                               |
| ------------------------------------------------------------------------------ |
| <mark style="background-color:yellow;">Eg: Xampp1(you can put any name)</mark> |

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

<mark style="color:purple;">**Step-by-Step Guide to**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">XAMPP</mark> <mark style="color:purple;"></mark><mark style="color:purple;">**Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`xampp`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `xampp1`
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
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an XAMPP instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 173602.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 173629.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 173706.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:blue;">FAQ</mark>

**About Xampp image we used.**

This image is maintained by the scale infinite.

**Do the image secure to use ?**

The image is created and verified by the scale infinite. it is a 100% secure image.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

#### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
