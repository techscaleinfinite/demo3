---
description: >-
  mStream transforms your home computer into a personal music streaming hub.
  Enjoy your music collection anywhere with mobile apps for Android and iPhone.
cover: ../../.gitbook/assets/download (7).png
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

# 📺 Mtream Deployment

### <mark style="color:blue;">What's Mstream?</mark>

<mark style="color:orange;">**mStream: Your Personal Symphony**</mark> <mark style="color:orange;"></mark><mark style="color:orange;">🎶</mark>

<mark style="color:orange;">Have you ever dreamed of having your very own music streaming server, where your cherished tunes are just a click away, no matter where you are? Well, enter mStream, the maestro of personal music streaming.</mark>

🏡 **Home is Where the Music Is** 🏡

With mStream, your home computer becomes the star of the show. It transforms your humble abode into a music hub, ready to serenade you with melodies from your own collection.

📱 **Music on the Move** 📱

But here's the kicker – mStream doesn't like to stay home all the time. It's a globetrotter, with mobile apps for both Android and iPhone. So, whether you're lounging on the couch or exploring far-off lands, your music library is right there in your pocket.

🌟 **Your Personal DJ** 🌟

Think of mStream as your personal DJ, spinning your favorite tracks with finesse. Its interface is as smooth as a dance floor, making navigation and playlists a breeze.

📡 **Anywhere, Anytime** 📡

With mStream, you're not confined to a single room or device. It breaks free from the shackles of location, bringing your music to any device with an internet connection. From your cozy den to a beachfront paradise, your playlist is your oyster.

🚀 **Stream with Confidence** 🚀

Security is key. mStream ensures that your music stays yours, protected behind digital fortifications. It's your vault, and only you hold the key.

So, if you're ready to turn your home into a music haven and your phone into a jukebox on-the-go, mStream is your backstage pass to an encore-worthy music streaming experience.

### <mark style="color:blue;">**How It Works:**</mark>

🎵 **Unveiling the Harmony: How mStream Works** 🎵

At the heart of mStream lies the magic of personal music streaming. Here's your backstage pass to the symphony:

🏡 **Home is Where the Soundwaves Begin** 🏡

mStream kicks off its performance right at home, on your trusty computer. It's here that your cherished music collection takes center stage.

📡 **The Connection That Knows No Bounds** 📡

But mStream isn't content with just staying indoors. It yearns to explore the world, and it does so through your mobile companions. There are apps, both for Android and iPhone, making sure your music is your travel companion.

🎶 **The Maestro Takes the Stage** 🎶

Picture mStream as your personal music maestro. It orchestrates your tunes effortlessly, curating playlists and making sure your music experience is pitch-perfect.

🌍 **Your Music, Your World** 🌍

The beauty of mStream? It's not tethered to one place. With an internet connection, it liberates your melodies, playing them on any device, wherever you roam.

🔒 **Security is Its Encore** 🔒

Safety is a top note for mStream. It ensures that your music fortress remains impenetrable, letting only you and your trusted audience listen in.

💫 **The Final Encore** 💫

So there you have it – mStream's secret sauce. It turns your home into a music sanctuary and your mobile into a pocket-sized concert hall. With mStream, music is more than sound; it's an experience.

Now, go on, let the music play, the world awaits your symphony

### <mark style="color:blue;">Steps And Procedure</mark>

<mark style="background-color:green;">**This deployment utilizes the official mstream Docker image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find the [linuxserver/mstream](https://hub.docker.com/r/linuxserver/mstream) application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the  mstream application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the mstream webpage and explore its content.

By following these straightforward steps, you'll have successfully deployed the  mstream application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------- |
| [`mstream`](https://hub.docker.com/r/linuxserver/mstream)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                               |
| ------------------------------------------------------------------------------ |
| <mark style="background-color:yellow;">Eg: mstram(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td>3000</td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

| Install with Default                                                                                                                                        | Advanced                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">(select this if you want install with default settings if don't have environment value and working directory)</mark> | <mark style="background-color:yellow;">(select this if you want to go with advanced settings, where you select you own environment value and working directory)</mark> |

If you choose Advanced option:

| ENV VARIABLE                                                            |
| ----------------------------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> |

| WORKING DIR                                                                                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p>                                                      |
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                                                                      |
| <p></p><pre class="language-yaml"><code class="lang-yaml">volumes:
      - /path/to/data:/config
      - /path/to/music:/music
</code></pre> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to mstream Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`mstream`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `mstream`
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
       * <mark style="color:red;">Here use ( use the path after   " :"  )</mark>
       *

           ```yaml
           volumes:
                 - /path/to/data:/config
                 - /path/to/music:/music
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an mstream instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-07 170759.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-07 170850.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About** mstream **image we used.**

This is the official mstream image.

**Can I deploy my own** mstream **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going/

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions&#x20;

</details>
