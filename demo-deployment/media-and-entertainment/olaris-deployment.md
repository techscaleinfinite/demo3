---
description: >-
  olaris is your creative hub for media management and transformation, driven by
  a passionate open-source community. Enjoy media curation, transcoding, and
  easy access with olaris-react.
cover: >-
  ../../.gitbook/assets/68747470733a2f2f692e696d6775722e636f6d2f65777a3554414e2e706e67.png
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

# 📺 Olaris Deployment

### <mark style="color:blue;">What's is olaris?</mark>

<mark style="color:orange;">Olaris is like a creative hub for media enthusiasts, a place where the community comes together to manage and transform their media treasures. At its heart lies the olaris-react project, the main interface that's here to streamline your media management experience. And, guess what? There are plans in the pipeline to support even more clients and applications down the road.</mark>

**Open-Source Community:** Olaris isn't just software; it's a labor of love, powered by a community that believes in the open-source spirit. It's like a collective art studio where everyone's brushes and talents come together to create something beautiful.

**Media Management:** Olaris is your digital curator, helping you organize, optimize, and enjoy your media collection. It's like having a personal archivist who ensures your media is always in its best form.

**Transcoding Wizardry:** Transforming media formats? Olaris has that covered too. It's like a magical spellcaster, turning your media into the perfect format for any occasion or device.

**Olaris-React:** At the forefront is olaris-react, your gateway to a world of media management possibilities. It's like a cozy library where you can easily browse through your media treasures and pick out just what you need.

**Community-Driven:** The best part? Olaris is not a solitary endeavor. It's a collaborative masterpiece crafted by a passionate community that understands the power of media. It's like a jam session where everyone's talents harmonize to create something extraordinary.

So, think of Olaris as your creative studio, your digital playground, and your media oasis—all rolled into one. It's the place where you and the community can make your media management dreams come true.

### <mark style="color:blue;">**How It Works:**</mark>

**Media Management:** Olaris provides a user-friendly web-based interface, like olaris-react, to make managing your media a breeze. It's like having a personal media assistant that helps you upload, organize, and manage all your media files, whether they're captivating videos, soul-soothing audio tracks, or cherished images. It's your digital command center for media organization.

**Transcoding:** Think of Olaris as your media magician. It's equipped with a transcoding engine that lets you perform media alchemy. You can transform your media files from one format to another, like turning a paperback into an e-book. Olaris allows you to specify all the details—output formats, codecs, bitrates, resolutions, and more. It's like having a studio where you can fine-tune your media to perfection, ready for any occasion or device.

**Server and Processing:** Olaris isn't just a pretty face; it's got the muscle too. It runs on a powerful server, which acts as the wizard behind the scenes. This server takes on the heavy lifting, handling all the grunt work of actual transcoding tasks. It's like having a dedicated production team backstage, making sure your media transformations happen seamlessly and without a hitch.

With Olaris, managing, transforming, and enjoying your media is a breeze. It's like having a trusted partner that not only understands your media needs but also has the skills and resources to make them a reality. Your media world becomes a place of order, creativity, and limitless possibilities

### <mark style="color:blue;">Steps And Procedure</mark>

&#x20; <mark style="background-color:purple;">**This deployment utilizes the official oalris Docker image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find the <mark style="color:orange;">olaristv/olaris-server</mark> application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the <mark style="color:orange;">olaris</mark> application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the  olaris webpage and explore its content.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------- |
| [olaris](https://hub.docker.com/r/olaristv/olaris-server)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                               |
| ------------------------------------------------------------------------------ |
| <mark style="background-color:yellow;">Eg: olaris(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td>8080</td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td></td></tr></tbody></table>

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
| /var/media                                                                              |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to olaris Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name: olaris</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: olaris
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: http
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
       * <mark style="color:red;">Here use ( use the path after   " :"  )</mark>
       * /var/media
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an HOMER instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div align="left">

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 124107.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 124324.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 125400.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 125906.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About olaris image we used.**

This is the official olaris image.

**Can I deploy my own olaris image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions&#x20;

</details>
