---
description: >-
  Radicale, your personal calendar and contact butler, effortlessly manages
  calendars, to-do lists, journal entries, and contacts. Setup is a breeze with
  Radicale, focusing on simplicity and efficiency.
cover: ../../.gitbook/assets/72caa053-radicle_logo.png
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

# 🖥 Radicale Deployment

### <mark style="color:blue;">What's is Radicale?</mark>

<mark style="color:orange;">**Your Personal Calendar and Contact Butler**</mark>

<mark style="color:orange;">Meet Radicale—the compact yet mighty server that's your go-to for all things calendars, to-do lists, and contacts. It doesn't just handle them; it masters the art of sharing and organizing effortlessly.</mark>

**Calendars, Todos, and More** Radicale has your back when it comes to keeping track of events, todos, journal entries, and those all-important business cards. It's a one-stop-shop for managing your personal and professional life.

**No Fuss, No Frills** Setting up Radicale is a breeze. Say goodbye to complicated configurations and endless setup steps. With Radicale, it's all about simplicity and efficiency. You'll be up and running in no time.

**Fort Knox for Your Data** Security is paramount, and Radicale gets that. You have control over who gets access to your calendars and contact lists. Only the authenticated ones get to peek inside.

**Data's Safe Haven** Radicale follows a simple yet robust approach—it stores all your valuable data neatly in a folder structure on your file system. No hidden corners or complex databases, just easy-to-navigate organization.

In a nutshell, Radicale is your personal assistant, handling calendars, to-do lists, and contacts with finesse. It's that reliable friend who ensures you're always on top of your game, never missing a beat. With Radicale, managing your life has never been this smooth. Give it a whirl and experience the ease of organized living.

### <mark style="color:blue;">**How It Works:**</mark>

<mark style="color:orange;">**How Radicale Works**</mark>

<mark style="color:orange;">Imagine having a trusty assistant for managing your calendars, to-do lists, and contacts. That's precisely what Radicale is—a smart, compact server that simplifies your life. Here's how it works:</mark>

**1. A Master of Sharing**

* Radicale supports CalDAV, CardDAV, and HTTP, making it a versatile tool for sharing calendars and contact lists.
* It effortlessly handles events, todos, journal entries, and business cards, ensuring all your data stays organized.

**2. Out-of-the-Box Convenience**

* No need to wrestle with complicated configurations. Radicale works seamlessly right from the get-go.
* It's designed for straightforward, hassle-free use.

**3. Your Data, Your Control**

* Radicale respects your privacy and security. You have the power to limit access through authentication.
* Your data is stored neatly in a user-friendly folder structure on your file system, giving you peace of mind.

In essence, Radicale is your personal data butler, efficiently managing your calendars, to-do lists, and contacts. It streamlines your life, ensuring you stay organized and in control. With Radicale, managing your data is not a chore; it's a breeze. Give it a try and experience the simplicity of Radicale for yourself.

### <mark style="color:blue;">Steps And Procedure</mark>

&#x20;<mark style="background-color:purple;">**This deployment utilizes the official radicale Docker image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find the  [tomsquest/docker-radicale](https://hub.docker.com/r/tomsquest/docker-radicale/) application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the radical  application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the  radical webpage and explore its content.

By following these straightforward steps, you'll have successfully deployed the radical application and gained access to its features through a seamless and user-friendly process.



### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                       |
| -------------------------------------------------------------------------------------------------------------------------------------------------- |
| r[adicale ](https://hub.docker.com/r/tomsquest/docker-radicale/)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                            |
| --------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: rad(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td>5232</td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                 |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to radicale Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name: radicale</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: radicale
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `5232`
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
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an radical instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-13 130518 (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-13 130244 (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/bbuu.png" alt=""><figcaption></figcaption></figure>

</div>

<div>

<figure><img src="../../.gitbook/assets/jhhjjjjjjjjjjjjjjjjjjjjjjjjjjjjjjjjjjjjj.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/mmmmmmm.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About** radical **image we used.**

This is the official radical image.

**Can I deploy my own** radical **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, radicale

</details>
