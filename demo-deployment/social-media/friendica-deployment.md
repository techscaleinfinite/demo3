---
cover: ../../.gitbook/assets/download.jpg
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

# Friendica Deployment

### <mark style="color:blue;">What's media wiki?</mark>

Friendica is a free and open-source social networking platform that provides a decentralized and federated alternative to commercial social media networks. Here's how Friendica works:

1. **User Registration:** Users can create accounts on Friendica servers, just like they would on traditional social media platforms.
2. **Decentralization:** Friendica is designed to be decentralized, meaning there's no central authority or corporation that controls the entire network. Instead, it operates on a federated model, similar to email. Users on one Friendica server can connect and interact with users on other Friendica servers.
3. **Federation Protocols:** Friendica uses federation protocols like ActivityPub, Diaspora, and OStatus to facilitate communication and interaction between different social networks and platforms. This enables users on Friendica to interact with users on other federated social networks.
4. **Profile and Content Creation:** Users can create profiles and share various types of content, including text posts, images, links, and videos. They can also customize their profiles, privacy settings, and notification preferences.
5. **Privacy and Control:** Friendica emphasizes user privacy and control over their data. Users can choose who can see their posts, and they have fine-grained control over their connections and interactions.
6. **Friendica Add-ons:** Friendica offers a range of add-ons and extensions that users can install to enhance their experience. These add-ons can include features like event calendars, file sharing, and more.
7. **Interactions:** Users can follow other users, send friend requests, and engage in conversations through comments, likes, and sharing. These interactions are typically visible to users' connections, depending on their chosen privacy settings.
8. **Cross-Platform Compatibility:** Friendica's federation protocols allow users to interact with users on different federated social networks. For example, a Friendica user can follow and communicate with someone on a different social network that also supports federation protocols.
9. **Hosting and Community:** Friendica can be self-hosted on private servers or hosted by community members. This flexibility allows users to choose their preferred level of control and privacy.
10. **Open Source:** Friendica is open-source software, which means its source code is freely available for anyone to inspect, modify, and contribute to. This transparency encourages community development and ensures that the platform remains free and open.

Overall, Friendica aims to provide a social networking experience that values user privacy, decentralization, and interoperability with other federated social networks. It offers an alternative to centralized social media platforms, allowing users to have more control over their online interactions and data.

### <mark style="color:blue;">**How It Works:**</mark>



1. **Decentralized Network:** Friendica operates on a decentralized network model. This means there is no single central server or authority controlling the entire network. Instead, Friendica instances, also known as nodes or pods, are independently operated by users or communities.
2. **Node Selection:** Users can choose to create their own Friendica instance or join an existing one. Each instance has its own set of users and can interact with other instances within the Friendica federation.
3. **User Registration:** To join Friendica, users need to register an account on their chosen instance. During registration, users provide a username, password, and email address. Some instances may have additional registration requirements or restrictions.
4. **Interoperability:** Friendica is designed to be compatible with other federated social networking platforms, such as Diaspora, Mastodon, and GNU Social. Users on Friendica can connect with users on these platforms, allowing for cross-network interactions.
5. **Profile Creation:** After registration, users can create their profile by adding personal information, profile pictures, and other details. They can also customize their privacy settings to control who can view their content.

### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official friendica Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the <mark style="color:orange;">friendica</mark>application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the friendica application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the friendica webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed the friendica application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------------------ |
| [`friendica`](https://hub.docker.com/\_/friendica)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                                 |
| -------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: friedika(you can put any name)</mark> |

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

<mark style="color:purple;">**Step-by-Step Guide to Friendica Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`friendica`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `friendica`
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

By following these steps, you can effortlessly deploy an Friendica instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-01 180241.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-01 180305.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-01 180401.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About** Friendica**image we used.**

This is the official Friendica image.

**Can I deploy my own** Friendica **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
