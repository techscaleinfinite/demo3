---
description: >-
  Grafana, an open-source analytics and visualization web application,
  transforms data into insights with interactive charts and data connectivity.
cover: ../../.gitbook/assets/grafana3182.jpg
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

# 💻 Grafana deployment

### <mark style="color:blue;">What's Grafana?</mark>

<mark style="color:orange;">**Grafana Unleashed: Your Data's Best Friend**</mark>

Meet Grafana, the Swiss Army knife of data analytics and visualization. It doesn't matter if you're a tech genius or just someone who loves numbers; Grafana is here to make data your best friend. Let's dive into what makes Grafana awesome:

<mark style="color:orange;">**Data Power Without Borders:**</mark> Grafana is your buddy across the board. Whether you're rocking a PC, Mac, or even a Raspberry Pi, it's got your back. No need to worry about compatibility—Grafana plays nice with everyone.

<mark style="color:orange;">**Where Open Meets Awesome:**</mark> Here's the cool part—it's open source. That means it's free, and everybody's invited to the party. You can tweak it, share it, and make it even cooler. Grafana is like an open playground where you're the boss.

<mark style="color:orange;">**Visualize Like a Pro:**</mark> Grafana is the Picasso of data. It takes your numbers and turns them into stunning charts and dashboards. No more squinting at endless rows of data; now you can see your trends and patterns in living color.

<mark style="color:orange;">**Data From Everywhere:**</mark> Grafana is a data detective. It connects to all your data sources, whether it's a database, an app, or something in the cloud. It's like having a data superhero that brings all your info under one roof.

<mark style="color:orange;">**Stay in the Know:**</mark> Grafana doesn't let you snooze. It's got this alert thingy that tells you when something's up. You set the rules, and when your data misbehaves, Grafana gives you a nudge. It's like having a personal data watchdog.

To sum it up, Grafana is the secret sauce to turn your data chaos into insights and high-fives. Whether you're a data pro or just dipping your toes, it's your ticket to understanding numbers like never before. Your data, your rules, your way!

### <mark style="color:blue;">**Working in Brief:**</mark>

\
<mark style="color:orange;">**Grafana: Your Data's Best Friend in Action**</mark>

Now that you've made friends with Grafana, let's see this buddy in action. Here's how it does its magic:

**1**<mark style="color:yellow;">**. The Data Detective:**</mark> Grafana can connect with just about any data source. Imagine it as the Sherlock Holmes of data, searching databases, cloud services, and APIs to gather clues (or in this case, data).

**2. **<mark style="color:orange;">**Creating Dashboards:**</mark> Grafana gives you the power to be the boss. You start by making your own dashboard. Think of it as a personal control center where you decide what data you want and how you want to see it.

**3**<mark style="color:yellow;">**. The Visual Artist**</mark>**:** Grafana is a true artist. It takes your data and transforms it into beautiful charts and graphs that respond to your every move. You click, it updates - real-time magic!

**4. **<mark style="color:orange;">**Stay in the Know:**</mark> It's like having a data babysitter. You tell Grafana what's important, and it keeps an eye on your data. If something goes wonky, it sends you a message. No more surprises.

**5. **<mark style="color:blue;">**Real-Time Wizard:**</mark> Grafana's visualizations are like a crystal ball for your data. You can see trends and changes as they happen. It's like having a data fortune-teller right at your fingertips.

In a nutshell, Grafana is your data sidekick, making the world of numbers and charts feel like a walk in the park. It's all about connecting, visualizing, and keeping you informed. Plus, it's open to all and keeps getting better with its cool community.

### <mark style="color:blue;">Steps And Procedure</mark>&#x20;

<mark style="background-color:purple;">**This deployment utilizes the official grafana Docker image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find the <mark style="color:orange;">grafana</mark> application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the <mark style="color:orange;">grafana</mark> application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the  <mark style="color:orange;">grafana</mark>  webpage and explore its content.

By following these straightforward steps, you'll have successfully deployed the <mark style="color:orange;">grafana</mark>  application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                            |
| --------------------------------------------------------------------------------------------------------------------------------------- |
| [`grafana`](https://hub.docker.com/r/grafana/grafana)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                                 |
| -------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: grafana1(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">80/3000</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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
| grafana-storage:/var/lib/grafana                                                        |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to Grafana Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`grafana`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `grafana1`
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
       * <mark style="color:red;">Here use ( use the path after   " :"  )</mark>
       * grafana-storage:/var/lib/grafana
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an GRAFANA instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 163652.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 164123.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/datasources (2).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/grafana-dashboard (1).png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:blue;">FAQ</mark>

**About grafana image we used.**

This is the official grafana image.

**Are there any restrictions on adding data sources ?**

you can add any data source that grafana supports.

**Can i deploy older version of grafana or my own modified grafana image ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, grafana

</details>
