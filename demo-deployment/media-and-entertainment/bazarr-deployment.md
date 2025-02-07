---
description: >-
  Bazarr, the unsung hero for your media, fetches tailored subtitles with
  personalization. Enjoy enhanced viewing with precise and fitting subtitles for
  your content.
cover: ../../.gitbook/assets/vsdj.png
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

# 📺 Bazarr Deployment

### <mark style="color:blue;">What's Bazarr?</mark>

<mark style="color:orange;">Bazarr is like a diligent wingman for your media, the unsung hero that makes sure every detail is perfect. It's the Robin to Sonarr and Radarr's Batman, focusing its superpowers on managing and fetching subtitles just the way you like them. Here's how Bazarr becomes your subtitle savior:</mark>

<mark style="color:orange;">**Subtitle Preferences:**</mark> Bazarr is all about personalization. You get to set your preferences for TV shows and movies, like choosing the perfect outfit for a special occasion. You tell Bazarr what you like, and it takes those preferences to heart.

<mark style="color:orange;">**Subtitle Hunting:**</mark> Once you've shared your preferences, <mark style="color:purple;">Bazarr</mark> goes on a quest. It tirelessly seeks out and downloads subtitles that match your media files, just like a trusty sidekick on a mission. It's as if it has a sixth sense for finding the exact right words.

<mark style="color:orange;">**Enhanced Viewing:**</mark> Thanks to Bazarr's dedication, your media viewing experience reaches new heights. You no longer have to squint at the screen or strain your ears to catch every word. Bazarr ensures that precise and fitting subtitles are always there to accompany your content, making every moment enjoyable.

In a world of media complexities, Bazarr is the friend who always has your back. It ensures that your favorite shows and movies are perfectly dressed in subtitles, ready to deliver an impeccable performance. Bazarr is the unsung hero that makes your media world a little more comfortable, a bit more magical, and a whole lot more enjoyable.

### <mark style="color:blue;">**How It Works:**</mark>

<mark style="color:orange;">**Integration**</mark>**:** Bazarr is your media companion that plays well with others. It seamlessly integrates with your media management software, like Sonarr for TV shows and Radarr for movies. Think of it as a friendly handshake between old pals who work together seamlessly.

<mark style="color:orange;">**Setting Preferences:**</mark> Bazarr respects your unique taste. It lets you set your subtitle preferences with meticulous detail. You can specify your language of choice, quality standards, preferred release groups, and more. It's like having your personal subtitle sommelier, ready to serve you the perfect pairing for your media.

<mark style="color:orange;">**Continuous Monitoring:**</mark> Bazarr is your vigilant guardian. It constantly keeps an eye on your media library, like a watchful sentry guarding a treasure trove. It's always on the lookout for new arrivals or changes.

<mark style="color:orange;">**Subtitle Search:**</mark> When new media enters your library, Bazarr springs into action. It becomes your diligent detective, combing through various subtitle provider websites like a seasoned investigator, searching for the elusive missing piece.

<mark style="color:orange;">**Download and Matching:**</mark> Once Bazarr finds suitable subtitles, it's like a skilled craftsman creating the final piece of a puzzle. It downloads the subtitles and carefully matches them with the corresponding media files in your library, ensuring they fit perfectly.

<mark style="color:orange;">**Notification**</mark>**:** Bazarr doesn't just work behind the scenes; it's polite enough to let you know when the job is done. It notifies your media management application, ensuring that the newly acquired subtitles become an integral part of your media metadata.

<mark style="color:orange;">**Automation:**</mark> The best part? It's all automated. You don't need to lift a finger. Bazarr takes care of the entire process, sparing you the hassle of manually searching and downloading subtitles for each and every media file. It's like having a trusty assistant who handles all the little details, leaving you to enjoy your media worry-free.

With Bazarr by your side, your media world becomes a place of convenience, personalization, and pure enjoyment. It's like having a reliable partner who anticipates your needs and makes sure your media experience is nothing short of perfect.

### <mark style="color:blue;">Steps And Procedure</mark>

<mark style="background-color:green;">**This deployment utilizes the official BAZARR Docker image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find the Bazarr application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the Bazarr application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the Bazarr webpage and explore its content.

By following these straightforward steps, you'll have successfully deployed the Bazarr application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                              |
| ----------------------------------------------------------------------------------------------------------------------------------------- |
| [`bazarr`](https://hub.docker.com/r/linuxserver/bazarr)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                                |
| ------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: bazarr1(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td>6767</td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

| Install with Default                                                                                                                                        | Advanced                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">(select this if you want install with default settings if don't have environment value and working directory)</mark> | <mark style="background-color:yellow;">(select this if you want to go with advanced settings, where you select you own environment value and working directory)</mark> |

If you choose Advanced option:

| ENV VARIABLE                                                            |
| ----------------------------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> |

| WORKING DIR                                                                                                                                                                           |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p>                                                                                               |
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                                                                                                               |
| <p></p><pre class="language-yaml"><code class="lang-yaml"> - /path/to/bazarr/config:/config
      - /path/to/movies:/movies #optional
      - /path/to/tv:/tv #optional
</code></pre> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to BAZARR Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`bazarr`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `bazar1`
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `6767`
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
            - /path/to/bazarr/config:/config
                 - /path/to/movies:/movies #optional
                 - /path/to/tv:/tv #optional
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an Bazarr instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 174403.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 174431.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 174523.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 174557.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About bazarr image we used.**

This is the official bazarr image.

**Can I deploy my own bazarr image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going.

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions , media, entertainment

</details>
