---
cover: ../../.gitbook/assets/Nextcloud_Logo.svg.png
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

# Next Cloud Deployment

### <mark style="color:blue;">What's Next cloud?</mark>

<mark style="color:orange;">"Nextcloud" is an open-source, self-hosted cloud storage and collaboration platform that allows you to store, sync, and share your files, documents, photos, and more. It provides a private and secure alternative to commercial cloud storage services.</mark>

### <mark style="color:blue;">**How It Works:**</mark>

**1. Installation and Setup:**

* You start by installing the Nextcloud software on a server or hosting provider of your choice. This server becomes your personal cloud storage platform.
* During the setup process, you create an admin account and configure basic settings.

**2. File Storage and Sync:**

* Nextcloud provides you with a central location to store your files, just like other cloud storage services. You can upload files, create folders, and organize your content.

**3. **<mark style="color:orange;">**File Synchronization:**</mark>

* Nextcloud offers synchronization clients for various platforms, including Windows, macOS, Linux, Android, and iOS. These clients keep your files synchronized across your devices, ensuring that the latest version of your files is available on all your devices.

**4. Sharing and Collaboration:**

* You can easily share files and folders with others using Nextcloud. You have the flexibility to share files publicly or with specific users, and you can set permissions for viewing, editing, or downloading.

### <mark style="color:blue;">Steps And Procedure</mark>

*   &#x20; <mark style="background-color:purple;">**This deployment utilizes the official NextCloud Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the <mark style="color:orange;">nextcloud</mark> application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the <mark style="color:orange;">nextcloud</mark> application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the  homer webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed the <mark style="color:orange;">nextcloud</mark> application and gained access to its features through a seamless and user-friendly process..

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                        |
| ----------------------------------------------------------------------------------------------------------------------------------- |
| [nextcloud](https://hub.docker.com/\_/nextcloud/)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                                                                                 |
| -------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg:</mark> nextcloud1<mark style="background-color:yellow;">(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td>8080</td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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

<mark style="color:purple;">**Step-by-Step Guide to nextcloud Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name: nextcloud</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: nextcloud
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: HTTP
   * Port: 8080
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

By following these steps, you can effortlessly deploy an nextcloud instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 160853.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 160919.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 161017.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About nextcloud image we used.**

This is the official nextcloud image.

**Can I deploy my own nextcloud image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
