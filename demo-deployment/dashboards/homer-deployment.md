---
description: >-
  Discover Homer, your user-friendly, self-hosted dashboard that simplifies
  managing various services and applications from a single, convenient
  interface, enhancing your productivity and accessibility.
cover: >-
  ../../.gitbook/assets/687474703a2f2f692e696d6775722e636f6d2f566958634741442e706e67.png
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

# 🖥 Homer Deployment

### <mark style="color:blue;">What's is homer?</mark>

_Homer is a user-friendly, self-hosted dashboard that simplifies the management of your various services and applications. This web-based dashboard offers quick and convenient access to a wide range of self-hosted tools and services from a single interface. It's designed to streamline your experience in organizing and interacting with your self-hosted applications, enhancing accessibility and productivity._

### <mark style="color:blue;">**How It Works:**</mark>

Homer simplifies the process of configuring and accessing your self-hosted services through these key steps:

1. _**Configuration**:_ Begin by defining the services you want to include in your Homer dashboard using a YAML configuration file. In this file, you list the names, URLs, and icons associated with each service you wish to access.
2. <mark style="color:blue;">**Dashboard Interface**</mark><mark style="color:blue;">:</mark> After setting up your configuration, you can access your Homer dashboard through a web browser. The dashboard offers an organized and user-friendly view of your services, making it straightforward to locate and launch them.
3. <mark style="color:yellow;">**Service Accessibility**</mark>: Each entry on the dashboard typically features an icon, a service name, and a URL link. Clicking on either the icon or the name of a service opens a new tab or window in your browser, taking you directly to the designated URL of that service.
4. <mark style="color:green;">**Customization**</mark><mark style="color:green;">:</mark> Homer goes the extra mile in terms of customization. You can personalize the appearance of your dashboard by selecting different themes, layouts, and colors that align with your preferences.
5. **Quick Access**: With Homer, there's no need to remember individual URLs or maintain a complex list of bookmarks for your self-hosted services. The dashboard provides a centralized hub, simplifying access to everything you need.

In essence, Homer transforms the way you interact with your self-hosted applications and services, offering a seamless and efficient solution for managing and accessing them all from a single, user-friendly interface.

### <mark style="color:blue;">Steps And Procedure</mark>

&#x20;<mark style="background-color:purple;">**This deployment utilizes the official Homer Docker image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find the <mark style="color:orange;">b4bz/homer</mark> application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the homer application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the  homer webpage and explore its content.

By following these straightforward steps, you'll have successfully deployed the homer application and gained access to its features through a seamless and user-friendly process.



### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------ |
| [homer](https://hub.docker.com/r/b4bz/homer)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                              |
| ----------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: homer(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">8080</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

| Install with Default                                                                                                                                        | Advanced                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">(select this if you want install with default settings if don't have environment value and working directory)</mark> | <mark style="background-color:yellow;">(select this if you want to go with advanced settings, where you select you own environment value and working directory)</mark> |

If you choose Advanced option:

| ENV VARIABLE                                                            |
| ----------------------------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> |

| WORKING DIR                                                                                                |
| ---------------------------------------------------------------------------------------------------------- |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p>                    |
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                                    |
| <p></p><pre class="language-bash"><code class="lang-bash">-v /path/to/appdata/config:/config
</code></pre> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to homer Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name: homer</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: homer
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `8080`
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
           -v /path/to/appdata/config:/config
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an HOMER instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 150802.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 150839.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About homer image we used.**

This is the official homer image.

**Can I deploy my own homer image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, homer

</details>
