---
description: >-
  Discover ZNC, your gateway to an enhanced IRC experience. Install and
  configure this versatile software to manage IRC connections with ease.
cover: ../../.gitbook/assets/znc.jpg
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

# 🖥 Znc Deployment

### <mark style="color:blue;">What's  Znc?</mark>

<mark style="color:orange;">ZNC serves as a vital component in the world of Internet Relay Chat (IRC), functioning as an IRC network bouncer, or more commonly known as a BNC. Its primary purpose is to introduce flexibility and convenience to the IRC experience.</mark>

### <mark style="color:blue;">**How It Works**</mark>

Here's a closer look at how ZNC operates:

1. **Installation and Setup:** To embark on the ZNC journey, users typically begin by installing and configuring the ZNC software on a server or host of their choosing. This serves as the foundation for their BNC service.
2. <mark style="color:yellow;">**IRC Connection:**</mark> ZNC acts as an intermediary between the IRC client and the IRC server. When an IRC client connects to the ZNC BNC, it essentially establishes a connection with ZNC, which subsequently connects to the chosen IRC server.
3. <mark style="color:purple;">**Detaching Clients:**</mark> One of the defining features of ZNC is its ability to detach clients. This means that once an IRC client connects to ZNC, it can gracefully disconnect from the IRC server without losing the ongoing conversations and channel memberships. ZNC keeps these connections active on behalf of the client.
4. **Channel Membership:** ZNC allows users to selectively detach from specific IRC channels while remaining connected to others. This enables users to focus on conversations of interest while temporarily detaching from channels that may be less relevant.
5. <mark style="color:green;">**Consolidation of Nicknames**</mark>**:** ZNC offers the valuable capability of consolidating multiple IRC clients from different locations into a single ZNC account. As a result, all these clients can appear under the same nickname on IRC, providing a unified presence to the IRC community.
6. <mark style="color:blue;">**Simultaneous Connections:**</mark> Users can connect multiple IRC clients to their ZNC account concurrently, even from different geographical locations. This simultaneous connection capability ensures that users can stay connected and participate in IRC discussions from various devices or locations.
7. <mark style="color:orange;">**Message Buffering:**</mark> ZNC's message buffering feature ensures that users do not miss out on conversations or messages that occurred while they were temporarily detached or disconnected. These messages are stored and made available when users reconnect.
8. **Security and Privacy:** ZNC prioritizes security and privacy. It often supports encryption and secure connections to ensure the confidentiality of communications. Users can also authenticate themselves securely with their ZNC instance.
9. <mark style="color:blue;">**Customization:**</mark> ZNC is known for its customization options. Users can configure and customize their ZNC setup to align with their preferences, including the choice of IRC servers, channels, and nicknames.
10. <mark style="color:green;">**User-Friendly Interface:**</mark> Many ZNC setups offer user-friendly web interfaces or command-line tools for configuration and management. This simplifies the process of controlling and monitoring the BNC.

In essence, ZNC enhances the IRC experience by allowing users to maintain a persistent presence on IRC networks while offering the flexibility to detach and reconnect at will. This makes it an indispensable tool for IRC enthusiasts, enabling them to manage their conversations and channel memberships seamlessly.

\


### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official ZNC Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the linuxserver/znc application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the ZNC application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the  ZNC webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed  ZNC application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                                         |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<mark style="color:orange;">ZNC</mark>](https://hub.docker.com/r/linuxserver/znc)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                            |
| --------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: znc(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">6501</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

| Install with Default                                                                                                                                        | Advanced                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">(select this if you want install with default settings if don't have environment value and working directory)</mark> | <mark style="background-color:yellow;">(select this if you want to go with advanced settings, where you select you own environment value and working directory)</mark> |

If you choose Advanced option:

| ENV VARIABLE                                                            |
| ----------------------------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> |

| WORKING DIR                                                                                                  |
| ------------------------------------------------------------------------------------------------------------ |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p>                      |
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                                      |
| <p></p><pre class="language-bash"><code class="lang-bash">-v /path/to/appdata/config:/config \
</code></pre> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to ZNC Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`ZNC`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `ZNC`
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `6501`
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

           ```bash
           -v /path/to/appdata/config:/config \
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an ZNC instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/ddd.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/bgbg.png" alt=""><figcaption></figcaption></figure>

</div>

<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-06 145501 (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-06 145526 (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/ggee.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About** ZNC **image we used.**

This is the official ZNC image.

**Can I deploy my own** ZNC **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, znc

</details>
