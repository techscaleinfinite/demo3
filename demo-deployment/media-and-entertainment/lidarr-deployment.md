---
description: >-
  Meet Lidarr, your music curator with tech brilliance. It scours Usenet and
  BitTorrent to find, sort, and upgrade your favorite music, ensuring your
  collection is always top-notch.
cover: ../../.gitbook/assets/lidarr.png
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

# 🎶 Lidarr Deployment

### <mark style="color:blue;">What's Lidarr?</mark>

<mark style="color:orange;">Picture this: you're a music enthusiast, and your collection is the crown jewel of your digital world. Now, imagine having a trusty sidekick named Lidarr, who's like your personal music curator with a dash of tech brilliance.</mark>

<mark style="color:red;">**Lidarr**</mark> isn't your ordinary music manager; it's a virtuoso in the world of Usenet and BitTorrent. It's got a keen eye on the horizon, constantly scanning multiple RSS feeds to hunt down new tracks from your favorite artists. And when it spots a gem, Lidarr doesn't just fetch it; it handles it with style.

Once Lidarr gets its hands on those musical treasures, it doesn't just toss them into the collection. No, no. It's got class. It sorts and renames them, giving your collection that polished, organized look. It's like having a personal butler for your music.

But Lidarr's talents don't stop there. It's not content with just any quality. When a better version of a track pops up on the scene, Lidarr is on it like a hawk. It'll automatically replace those older files with the shiny, new, high-quality ones, keeping your collection top-notch.

Think of Lidarr as your music-savvy friend who always knows where to find the latest tunes and how to keep your collection in tip-top shape. So, whether you're a music connoisseur or just a casual listener, Lidarr is your backstage pass to music management nirvana.

### <mark style="color:blue;">**How It Works:**</mark>

<mark style="color:orange;">Certainly, let's unravel the magic behind</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**Lidarr**</mark> <mark style="color:orange;"></mark><mark style="color:orange;">in a way that's as unique as its abilities!</mark>

**Lidarr** is like your personal DJ on a mission to upgrade your music game. It works its charm by tapping into the world of Usenet and BitTorrent, which is where all the musical secrets are hidden.

🎵 <mark style="color:purple;">**Step 1: The Music Radar**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">🎵</mark>

Lidarr has an impeccable taste in music; it knows your favorite artists like the back of its digital hand. It scours the vast landscape of RSS feeds, keeping a vigilant watch for any new tracks these maestros drop. When it spots a musical treasure, it's like Lidarr's version of a musical jackpot!

🎶 <mark style="color:yellow;">**Step 2: The Organizing Virtuoso**</mark> <mark style="color:yellow;"></mark><mark style="color:yellow;">🎶</mark>

But Lidarr isn't just about collecting music; it's all about presentation. It doesn't just toss those tracks into your collection willy-nilly. Oh no, that's not its style. Lidarr takes those musical gems and gives them a proper place in your library. It's like having a personal butler for your tunes, making sure everything is neat, tidy, and easy to find.

🌟 <mark style="color:purple;">**Step 3: The Quality Maestro**</mark> 🌟

Lidarr is all about quality, darlings. When it stumbles upon a better version of a track you already have, it's on it like a star on the Hollywood Walk of Fame. It'll automatically replace those older files with the high-quality, pristine ones, making sure your collection always sounds like a million bucks.

So, think of Lidarr as your music-savvy best friend, always in the know about the latest hits and dedicated to keeping your music collection in top-notch shape. With Lidarr, your music library isn't just a bunch of files; it's a symphony of organization and excellence!

### <mark style="color:blue;">Steps And Procedure</mark>

<mark style="background-color:green;">**This deployment utilizes the official LIDARR Docker image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find the linuxserver/lidarr application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the Lidarr application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the Lidarr webpage and explore its content.

By following these straightforward steps, you'll have successfully deployed the Lidarr application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                                                           |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [L](https://hub.docker.com/r/linuxserver/lidarr)i[dar](https://hub.docker.com/r/linuxserver/lidarr)r<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                               |
| ------------------------------------------------------------------------------ |
| <mark style="background-color:yellow;">Eg: LIADRR(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td>8686</td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

| Install with Default                                                                                                                                        | Advanced                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">(select this if you want install with default settings if don't have environment value and working directory)</mark> | <mark style="background-color:yellow;">(select this if you want to go with advanced settings, where you select you own environment value and working directory)</mark> |

If you choose Advanced option:

| ENV VARIABLE                                                            |
| ----------------------------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> |

| WORKING DIR                                                                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p>                                                                                                            |
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                                                                                                                            |
| <p></p><pre class="language-yaml"><code class="lang-yaml"> - /path/to/appdata/config:/config
      - /path/to/music:/music #optional
      - /path/to/downloads:/downloads #optional
</code></pre> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to lidar Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`lidarr`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `liadrr`
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `8686`
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
            - /path/to/appdata/config:/config
                 - /path/to/music:/music #optional
                 - /path/to/downloads:/downloads #optional
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an LIADRR instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-07 143032.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-07 143209.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-07 143151.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About** LIADRR **image we used.**

This is the official LIADRR image.

**Can I deploy my own** LIADRR **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions&#x20;

</details>
