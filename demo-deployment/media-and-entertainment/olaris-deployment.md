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

<mark style="color:blue;">**olari-react:**</mark> The Heart of the Experience

At the core of Olaris is the olaris-react project, your trusty companion in the realm of media management. This interface is your ticket to a smoother and more enjoyable experience when handling your media. And guess what? We're cooking up exciting plans to support even more clients and applications in the near future, so stay tuned!

<mark style="color:orange;">**The Open-Source Art Studio**</mark>

Olaris is not just a piece of software; it's a collective labor of love, driven by a vibrant community that celebrates the open-source spirit. It's like a bustling art studio, where everyone's brushes and talents converge to create something truly beautiful.

<mark style="color:orange;">**Your Digital Curator**</mark>

Picture Olaris as your very own digital curator, tirelessly working to organize, optimize, and enhance your media collection. It's like having a personal archivist who ensures that your media is always in its prime.

<mark style="color:orange;">**Media Format Sorcery**</mark>

Need to work magic on media formats? Olaris has got you covered. It's like a wizard casting spells, effortlessly transforming your media into the perfect format for any occasion or device.

<mark style="color:orange;">**olari-react: Your Gateway**</mark>

Leading the charge is olari-react, your gateway to a world of media management possibilities. Think of it as your cozy library, where you can effortlessly browse through your media treasures and pick out exactly what you need.

<mark style="color:orange;">**A Symphony of Community**</mark>

But here's the best part: Olaris isn't a solo act. It's a collaborative masterpiece, forged by a passionate community that understands the immense power of media. It's like a jam session where everyone's talents harmonize to create something truly extraordinary.

So, envision Olaris as your creative studio, your digital playground, and your sanctuary for all things media. It's where you and the community can turn your wildest media management dreams into reality. Welcome to the future of media management—welcome to Olaris.

### <mark style="color:blue;">**How It Works:**</mark>

Are you curious about the inner workings of Olaris, your digital haven for media management? Let's dive in and unveil the magic behind the scenes.

<mark style="color:orange;">**Media Management Made Easy**</mark>

At the heart of Olaris is a user-friendly web-based interface, such as the ever-capable olaris-react. Think of it as your personal media assistant, tirelessly working to streamline your media management experience. Upload, organize, and manage all your media files with ease, whether they're captivating videos, soul-soothing audio tracks, or cherished images. It's your digital command center for all things media organization.

<mark style="color:orange;">**Transcoding: The Media Alchemy**</mark>

Olaris is your go-to media magician, equipped with a transcoding engine that performs media alchemy. Imagine turning a paperback into an e-book—it's that simple. Specify all the details you desire, from output formats and codecs to bitrates and resolutions. Olaris is like having a high-tech studio where you can fine-tune your media to perfection, making it ready for any occasion or device.

<mark style="color:orange;">**The Powerhouse Behind the Curtain**</mark>

But Olaris isn't all style and no substance. It operates on a robust server that acts as the wizard working behind the scenes. This server takes on the heavy lifting, handling all the grunt work of actual transcoding tasks. It's akin to having a dedicated production team backstage, ensuring your media transformations happen seamlessly and without a hitch.

With Olaris, managing, transforming, and enjoying your media becomes a seamless and delightful experience. It's like having a trusted partner that not only understands your media needs but also possesses the skills and resources to bring them to life. Your media world transforms into a realm of order, creativity, and limitless possibilities.

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

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, media, entertainment, olaris

</details>
