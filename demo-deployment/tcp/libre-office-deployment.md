---
cover: >-
  ../../.gitbook/assets/06ajIYT7R4AM7Fx9S9aUmBn-14.fit_lim.size_1050x591.v1613661897.png
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

# 📜 Libre Office Deployment

### <mark style="color:blue;">What's  libre office?</mark>

LibreOffice is like that versatile Swiss Army knife of office software, but in the digital realm. It's a suite of applications that roll up their sleeves and handle your document, spreadsheet, and presentation needs with finesse, all while keeping your wallet happy because it's open-source and free.

Picture this: You've got a report to write, a spreadsheet to crunch numbers in, and a presentation to woo your audience. Instead of juggling different tools, LibreOffice steps in as your trusty sidekick, offering Writer for your text, Calc for those complex calculations, and Impress to make your ideas pop.

It's not just about practicality; it's about freedom. LibreOffice doesn't tie you down with licenses or subscriptions; it's an open book, allowing you to explore, modify, and share it with your fellow digital adventurers.

And here's the fun part: It's a bit like that magical wardrobe from Narnia. You open it up, and suddenly, you're in a world of creativity and productivity, with tools that feel familiar, user-friendly, and ready to help you conquer that next document, spreadsheet, or presentation challenge.

### <mark style="color:blue;">**How It Works:**</mark>

Alright, let's dive into the enchanting world of LibreOffice and see how this versatile suite of office applications works its magic.

**Imagine you've got a document to create**. You fire up LibreOffice Writer, which is like your trusty word processor. You type away, add some stylish formatting, insert images, and create a masterpiece. Behind the scenes, LibreOffice uses its open-source wizardry to handle the text, layout, and even spell-checking, making your words look as sharp as a well-tailored suit.

**Now, let's talk numbers.** You need to crunch some data for that important project. LibreOffice Calc steps in as your spreadsheet wizard. You enter your numbers, create formulas, and watch it perform mathematical feats. It's like having a mathematical butler who's always on point.

<mark style="color:orange;">**But what about that upcoming presentation?**</mark> LibreOffice Impress is your ticket to creating captivating slides. You add text, images, charts, and transitions. When you hit "play," it's showtime! Your audience will be nodding in agreement, and they won't even realize it's your secret weapon.

**The beauty of LibreOffice lies in its open-source nature.** It's not some locked-up, proprietary software; it's a collaborative playground. Developers from around the globe have chipped in to make it user-friendly, flexible, and free. It's a bit like an open book; you can read, write, and share your own stories.

So, in a nutshell, LibreOffice works by giving you the tools you need to create, calculate, and captivate without the hassle of expensive licenses. It's the friendly neighborhood superhero of office software, making your digital tasks a breeze.\


### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official LIBRE OFFICE Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the linuxserver/libreoffice application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the libreoffice application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the libreoffice webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed  libreoffice application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                      |
| ------------------------------------------------------------------------------------------------------------------------------------------------- |
| [LIBREOFFICE](https://hub.docker.com/r/linuxserver/libreoffice)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                                    |
| ----------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: LIBREOFFICE(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">3000</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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

<mark style="color:purple;">**Step-by-Step Guide to LIBREOFFICE Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`libreoffice`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: libreoffice
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `3000`
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

By following these steps, you can effortlessly deploy an  libreoffice instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-07 112726.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-07 112743.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-07 115552.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-07 115446.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-07 115340.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About** libreoffice **image we used.**

This is the official libreoffice  image.

**Can I deploy my own** libreoffice **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
