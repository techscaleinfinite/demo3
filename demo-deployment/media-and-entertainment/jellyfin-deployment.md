---
description: >-
  Jellyfin, your open-source media maestro, effortlessly organizes and streams
  your diverse media collection. Enjoy freedom, media variety, device
  compatibility, and personalized customization.
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

# 📺 Jellyfin Deployment

### <mark style="color:blue;">What's Jellyfin?</mark>

<mark style="color:orange;">**Jellyfin: Your Personal Media Maestro**</mark>

<mark style="color:orange;">**A Symphony of Media Freedom:**</mark> Jellyfin is like an open-air concert for your media. It's open-source, meaning it's free for all to enjoy. You get a powerful platform to organize and stream your personal media without reaching for your wallet.

<mark style="color:orange;">**Media Wonderland:**</mark> Whether you're a movie buff, a music lover, or a photography enthusiast, Jellyfin's got your back. It plays nicely with all sorts of media, from your favorite songs to cherished videos and treasured photos.

<mark style="color:orange;">**Your Media, Your Way:**</mark> With Jellyfin, your media is wherever you are. It harmoniously streams your content to a variety of devices, ensuring you can dive into your collection no matter what gadget you're using.

<mark style="color:orange;">**Tailored to You:**</mark> Personalization is Jellyfin's middle name. You can customize your media server's look and feel to match your style. It's like having your own private media den, designed just the way you like it.

<mark style="color:orange;">**Fort Knox for Your Media:**</mark> Worried about privacy? Jellyfin has you covered. Since it's self-hosted, there's no need to fret about nosy neighbors. It's like having a safe vault for your digital treasures.

In a world where media reigns supreme, Jellyfin is your media maestro. It ensures your collection is neat, accessible, and completely under your command. Think of it as your personal media curator, ready to serve entertainment whenever and wherever you want it.

### <mark style="color:blue;">**Working in Brief:**</mark>

<mark style="color:orange;">**Media Library Zen**</mark>**:** Think of Jellyfin as your personal librarian for all things media. It takes your movies, music, and more and neatly organizes them by type, genre, or artist. It's like having a beautifully sorted bookshelf for your entertainment collection.

<mark style="color:orange;">**Entertainment on Demand:**</mark> Jellyfin plays the role of a magical genie, granting your media wishes on demand. It effortlessly streams your media to your devices, no matter if they're in your living room or on the other side of the world.

<mark style="color:orange;">**VIP Access:**</mark> With Jellyfin, your media kingdom becomes exclusive. You simply log in to your Jellyfin account for a tailored experience. It's like having a VIP pass to your personal media wonderland.

<mark style="color:orange;">**Media Multilingualism:**</mark> Jellyfin is the ultimate linguist for your media. It can translate media formats in real-time to match your devices, ensuring everything plays smoothly. It's like having a universal remote control for your media.

<mark style="color:orange;">**Worldwide Entertainment:**</mark> Jellyfin opens the door to a world of media. You can enjoy your collection from anywhere, as if you're carrying your entire media library in your pocket. It's ready to entertain you wherever you go.

Jellyfin takes the complexity out of managing your media. It puts you in charge of your entertainment kingdom with its self-hosted solution, and since it's open-source, you have the keys to customize it as you like. With Jellyfin, your media remains private and secure, promising an entertainment experience that's uniquely yours.

### <mark style="color:blue;">Steps And Procedure</mark>

&#x20; <mark style="background-color:purple;">**This deployment utilizes the official jellyfin Docker image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find the <mark style="color:orange;">jellyfin</mark> application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the <mark style="color:orange;">jellyfin</mark> application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the  <mark style="color:orange;">jellyfin</mark> webpage and explore its content.

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
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                 |
| <p>-v /path/to/tvseries:/data/tvshows<br>-v /path/to/movies:/data/movies</p>            |

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
       * <mark style="color:red;">Here use ( use the path after   " :"  )</mark>
       * \-v /path/to/tvseries:/data/tvshows\
         \-v /path/to/movies:/data/movies
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy and JELLY instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/kkk.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/ffb.png" alt=""><figcaption></figcaption></figure>

</div>

<div>

<figure><img src="../../.gitbook/assets/hhhh.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/fhhhhk.png" alt=""><figcaption></figcaption></figure>

</div>

<div>

<figure><img src="../../.gitbook/assets/gggggnm.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/llp (1).png" alt=""><figcaption></figcaption></figure>

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

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, media, entertainment, jellyfin

</details>
