---
description: >-
  Meet Gatus, your multi-talented health dashboard and digital Sherlock Holmes.
  It monitors various services, evaluates conditions, and serenades you with
  real-time insights for your digital kingdom.
cover: ../../.gitbook/assets/banwagongcncom_gatus_logo.png
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

# 📊 Gatus Deployment

### <mark style="color:blue;">What's  Gatus?</mark>



<mark style="color:orange;">**Gatus: Your Health Dashboard Maestro**</mark>

<mark style="color:orange;">Imagine having a trusty health dashboard that not only monitors your digital kingdom but also serenades you with real-time insights. Meet Gatus, the developer's secret weapon for keeping a watchful eye on services.</mark>

**Multi-Talented Monitoring:** Gatus wears many hats. It's your health dashboard for HTTP, ICMP, TCP, and even DNS queries. It's like having a Swiss Army knife for service evaluation.

**Condition Maestro:** Gatus isn't just a spectator; it's a judge of service health. It evaluates conditions like status codes, response times, certificate expirations, and even inspects the body of responses. It's the Sherlock Holmes of digital health checks.

**Alerting Virtuoso:** Gatus doesn't just detect issues; it knows how to make a scene. Pair your health checks with alerts that play a symphony of notifications through Slack, PagerDuty, Pushover, Discord, Twilio, and more. It's like having your own orchestra conductor for service disruptions.

**Versatile and Adaptable:** Like a chameleon, Gatus adapts to your needs. Whether you're guarding web services, databases, or other critical components, it's a vigilant sentry that you can configure to suit your environment.

**User-Friendly Baton:** Gatus's user interface is a friendly maestro's baton, allowing you to compose your monitoring symphony with ease. It's an intuitive conductor's wand for orchestrating your checks.

**Detailed Insights:** Gatus doesn't just nod at issues; it provides detailed insights. Dive into response data, error codes, and trends to conduct a thorough diagnosis of your services.

**Open Source Orchestra:** Behind Gatus's curtains is an open-source orchestra of contributors. It's a global ensemble of developers and sysadmins collaborating to fine-tune the health-check symphony.

**Cross-Channel Communication:** Gatus isn't shy about delivering messages. Whether you prefer Slack's chat, PagerDuty's alerts, or Twilio's SMS, it ensures that you're always in the know.

**Data-Driven Decisions:** With Gatus by your side, you make data-driven decisions. It's like having a crystal ball that foretells issues before they disrupt your digital realm.

**Soothing the Tech-Savvy Soul:** In the realm of health dashboards, Gatus is the soothing ballad for the tech-savvy soul. It's your conductor, your judge, and your sentinel—all in one.nd as speedy as Usain Bolt. It's your trusty sidekick in the ever-watchful world of online monitoring!

### <mark style="color:blue;">**How It Works:**</mark>

<mark style="color:orange;">**How Gatus Works: The Symphony of Service Health**</mark>

<mark style="color:orange;">Imagine Gatus as the conductor of your service health orchestra. It orchestrates the harmony of monitoring and alerting in a truly unique way.</mark>

1. **Monitoring Mastery**: Gatus sweeps the stage, monitoring your services with a range of queries: HTTP, ICMP, TCP, and DNS. It's like having a virtuoso who can play any instrument in the orchestra.
2. **Condition Evaluation**: This conductor doesn't just listen; it evaluates each performance rigorously. It checks the status code, response time, certificate expiration, and even the body of responses. It's like having a keen-eyed music critic for your services.
3. **Alerting Overture**: Gatus doesn't stop at detection; it's the maestro of alerting. Pair your health checks with alerts that can harmonize through Slack, PagerDuty, Pushover, Discord, Twilio, and more. It's like having an entire symphony of notification methods at your disposal.
4. **Adaptability Encore**: Just like a seasoned conductor adjusts the tempo, Gatus adapts to your unique needs. It can guard web services, databases, and other critical components with ease. It's the versatile conductor who knows every musical genre.
5. **User-Friendly Baton**: Gatus wields a user-friendly interface, making it simple to compose your monitoring symphony. It's like having an intuitive conductor's baton in hand, ready to guide your checks.
6. **Detailed Composition**: Gatus doesn't skim over issues; it dives deep into the score. Explore response data, error codes, and trends for a comprehensive diagnosis of your services. It's like having the sheet music to every note played.
7. **Open-Source Orchestra**: Behind Gatus's curtain is a global ensemble of developers and sysadmins, collaborating to fine-tune the health-check symphony. It's an open-source orchestra, welcoming contributions from around the world.
8. **Cross-Channel Performance**: Gatus knows how to communicate. Whether it's the casual chat of Slack, the urgency of PagerDuty's alerts, or the directness of Twilio's SMS, it ensures you hear every note.
9. **Data-Driven Crescendo**: With Gatus, your decisions crescendo into data-driven masterpieces. It's like having a crystal ball that reveals issues before they become disruptive solos in your digital realm.
10. **Soothing the Tech-Savvy Soul**: In the realm of health dashboards, Gatus is the soothing ballad for the tech-savvy soul. It's your conductor, your critic, and your guardian—an all-in-one symphony of service health.

Gatus conducts your service health with precision, ensuring that your digital orchestra always plays in tune.\


### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official  gatus Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the [twinproduction/gatus](https://hub.docker.com/r/twinproduction/gatus) application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the  gatus application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the gatus webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed   gatus application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                             |
| ---------------------------------------------------------------------------------------------------------------------------------------- |
| [gatus](https://hub.docker.com/r/twinproduction/gatus)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                              |
| ----------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: gatus(you can put any name)</mark> |

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
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                 |
| --mount type=bind,source="$(pwd)"/config.yaml,target=/config/config.yaml                |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to gatus Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark><mark style="color:orange;">`gatus`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: gatus
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
       * \--mount type=bind,source="$(pwd)"/config.yaml,target=/config/config.yaml
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an  gatus instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-07 175302.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-07 175355.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-07 175331.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About**  uptime gatus**image we used.**

This is the official uptime gatus image.

**Can I deploy my own** uptime gatus **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions&#x20;

</details>
