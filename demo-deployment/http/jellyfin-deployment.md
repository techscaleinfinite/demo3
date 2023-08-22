---
cover: ../../.gitbook/assets/download (1).png
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

# Jellyfin Deployment

### <mark style="color:blue;">What's Jellyfin?</mark>

Jellyfin is a versatile, open-source media server software designed to help users organize, manage, and stream their personal media collection, including music, videos, and pictures, across a range of devices.

**Key Points:**

1. <mark style="color:orange;">**Open-Source Media Server**</mark>**:** Jellyfin is freely accessible, providing a platform to organize and stream personal media.
2. **Media Variety:** It supports various types of media, from music tracks to videos and images.
3. <mark style="color:orange;">**Device Compatibility**</mark>**:** Jellyfin streams content to a wide array of devices, ensuring seamless access.
4. **Customization:** Tailor your media server's interface and functionality to suit your preferences.
5. <mark style="color:orange;">**User Privacy**</mark>**:** Your media collection remains private as it's self-hosted, with no external sharing.

### <mark style="color:blue;">**Working in Brief:**</mark>

1. **Media Organization:** Jellyfin catalogues your media library, allowing you to arrange content by type, genre, or artist.
2. <mark style="color:orange;">**Streaming Capability**</mark>**:** Upon request, Jellyfin streams media to connected devices over a local network or the internet.
3. **User Authentication:** Users log in to their Jellyfin accounts to access their personalized media libraries.
4. <mark style="color:orange;">**Transcoding & Formats**</mark>**:** Jellyfin adapts media formats for compatibility with different devices.
5. **Remote Access:** Enjoy your media on-the-go by accessing your Jellyfin server from external locations.

Jellyfin simplifies media management, offering a self-hosted solution for streaming your favorite content across various devices. Its open-source nature empowers customization and ensures that your media remains private and secure.

### <mark style="color:blue;">Steps And Procedure</mark>

* &#x20;<mark style="background-color:yellow;">**This deployment uses the linuxserver/jellyfin Docker image**</mark>**.**
* &#x20;Go to create apps page and Search <mark style="color:orange;">linuxserver/jellyfin</mark> on the search bar.
* &#x20;Click on install button.
* &#x20;Fill all the required fields.
* click on Advanced.
* Default Installation is enough for Jellyfin to be up and running. Click install
* You will be redirected to My Apps page, Here you can find all the applications you deployed.
* &#x20;Copy the Jellyfin application Hostname without NodePort and search the Url.
* &#x20;Now you will access the application. And start setting up the application.
* &#x20;Now Follow the on screen instructions and setup your account
* &#x20;We’ll add media files using ftp
* &#x20;Goto SFTP section in right-side bar menu and click 'Reinitilze password'
* &#x20;You will get credentials to login to your sftp storage. SFTP storage can be accessed using various tools, example:- Filezilla
* Select HDD to Server
* &#x20;Make sure you have provided right From and To file paths
* &#x20;Add the uploaded media files into the jellyfin using its web interface

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                               |
| ------------------------------------------------------------------------------------------------------------------------------------------ |
| [`Jellyfin`](https://hub.docker.com/r/jellyfin/jellyfin)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                              |
| ----------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: jelly(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">8096</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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

<mark style="color:purple;">**Step-by-Step Guide to jellyfin Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`jellyfin`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `jelly`
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `8096`
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

By following these steps, you can effortlessly deploy and JELLY instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 161711.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 161749.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 161854.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 161922.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 162015.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 162055.png" alt=""><figcaption></figcaption></figure>

</div>



### <mark style="color:blue;">FAQ</mark>

**About Jellyfin image we used.**

This is the official linuxserver/jellyfin image.

**Are there any restrictions on adding data sources ?**

you can add any data source that Jellyfin supports.

**Can i deploy older version of Jellyfin or my own modified Jellyfin image ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
