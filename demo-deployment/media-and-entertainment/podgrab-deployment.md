---
description: >-
  Podgrab: Your personal podcast sidekick. Discover, download, and enjoy
  podcasts effortlessly with auto-downloads and simple podcast discovery. Your
  podcast, your way.
cover: >-
  ../../.gitbook/assets/pngtree-podcast-icon-vector-design-radio-broadcasting-or-streaming-vector-stock-illustration-png-image_2154579.jpg
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

# 🎵 Podgrab Deployment

### <mark style="color:blue;">What's podgrab?</mark>

<mark style="color:orange;">Podgrab: Your Podcast Sidekick for Effortless Listening</mark>

<mark style="color:orange;">Discovering, downloading, and enjoying your favorite podcasts has never been easier, thanks to Podgrab. This self-hosted podcast manager is your ticket to a seamless and enjoyable podcasting experience. Let's dive into the world of Podgrab and explore how it elevates your podcast game.</mark>

**Auto-Download Magic:** Imagine waking up, grabbing your morning coffee, and voila! Podgrab has already downloaded the latest episodes of your favorite podcasts. It's like magic. With Podgrab, you can set it and forget it, knowing that your podcasts will be ready to accompany you on your daily adventures.

**Podcast Discovery Made Simple:** Looking for new podcasts to love? Podgrab has your back. It seamlessly connects with the iTunes API, making it a breeze to search for and add podcasts. Whether you're into storytelling, education, or comedy, there's a podcast waiting for you to discover.

**Your Podcast Player, Your Rules:** Podgrab isn't just about downloading; it's a full-fledged podcast player. Play your downloaded episodes or stream them directly from the original source—it's your call. With Podgrab, you're in control of your podcast listening experience.

**Diverse Adding Options:** Adding podcasts is a piece of cake with Podgrab. You can do it the classic way by entering a direct RSS feed URL, import your subscriptions via OMPL, or simply search and add using keywords. Flexibility is the name of the game here.

**Keep Your Collection Organized:** Worried about running out of storage space? Don't be. Podgrab is smart enough to detect existing episode files, preventing unnecessary re-downloads. You'll never have to stress about duplicate files cluttering your storage.

**Customizable Episode Names:** Want to add a personal touch to your episodes? Customize their names to your heart's content. Make them memorable, fun, or organized—whatever suits your style.

**Dark Mode for Night Owls:** For those late-night listening sessions, Podgrab offers a sleek dark mode. It's easy on the eyes and sets the mood for an immersive podcast exploration.

**Self-Hosted and Open Source:** With Podgrab, you're in control. It's self-hosted, which means your podcast data stays with you. Plus, it's open source, fostering a community of podcast enthusiasts who continually enhance the platform.

In a nutshell, Podgrab is your dedicated podcast sidekick, simplifying the way you discover, download, and enjoy podcasts. It's your gateway to an organized, personalized, and delightful podcasting journey. So, what are you waiting for? Let Podgrab transform your podcast experience today!

### <mark style="color:blue;">**How It Works:**</mark>

* **Auto-Download Magic:** Picture this: You wake up, and your favorite podcasts are already there, waiting for you. Thanks to Podgrab's auto-download feature, it fetches the latest episodes automatically, keeping you in the loop effortlessly.
* **Podcast Discovery Made Simple:** Discovering new podcasts is a walk in the park with Podgrab. Its seamless integration with the iTunes API lets you search for and add podcasts that catch your eye. No more hunting around; Podgrab makes discovery a breeze.
* **Your Podcast Player, Your Rules:** Podgrab isn't just about downloading; it's a full-fledged podcast player. You have the power to choose—play your downloaded episodes or stream them directly from the source. With Podgrab, your podcast experience is in your hands.
* **Diverse Adding Options:** Adding podcasts is flexible with Podgrab. You can go old-school by entering a direct RSS feed URL, bring in your subscriptions via OMPL, or keep it simple by searching and adding using keywords. The choice is yours.
* **Keep Your Collection Organized:** Concerned about running out of storage space? Fear not. Podgrab is clever enough to spot existing episode files, so you won't end up with duplicates cluttering your device. Say goodbye to storage headaches.
* **OPML Made Easy:** For those with extensive podcast libraries, Podgrab offers effortless OPML import/export. Share your podcast lineup across devices or with fellow enthusiasts hassle-free.
* **Customizable Episode Names:** Want to add a personal touch? Customize episode names to your liking. Make them memorable, witty, or simply well-organized—Podgrab adapts to your style.
* **Dark Mode for Night Owls:** Late-night podcast sessions? No problem. Podgrab's sleek dark mode is easy on the eyes, creating the perfect ambiance for immersive listening.
* **Self-Hosted and Open Source:** With Podgrab, you're in control. It's self-hosted, meaning your podcast data stays securely with you. Plus, it's open source, fostering a community of podcast lovers who continually enhance the platform.

In a nutshell, Podgrab is your trusty podcast companion, simplifying the way you discover, download, and enjoy podcasts. It's your passport to an organized, personalized, and delightful experience.

### <mark style="color:blue;">Steps And Procedure</mark>

<mark style="background-color:green;">**This deployment utilizes the official podgrab Docker image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find the [akhilrex/podgrab](https://hub.docker.com/r/akhilrex/podgrab/) application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the  Podgrab application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the Podgrab webpage and explore its content.

By following these straightforward steps, you'll have successfully deployed the  Podgrab application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                              |
| ----------------------------------------------------------------------------------------------------------------------------------------- |
| [`podgrab`](https://hub.docker.com/r/akhilrex/podgrab/)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                                |
| ------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: podgrab(you can put any name)</mark> |

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

| WORKING DIR                                                                                      |
| ------------------------------------------------------------------------------------------------ |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p>          |
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                          |
| <p></p><pre class="language-sh"><code class="lang-sh">/host/path/to/assets:/assets
</code></pre> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to podgrab Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`podgrab`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `Podgrab`
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
       *

           ```sh
           /host/path/to/assets:/assets
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an  Podgrab instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/fgfgf.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/ghgh.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/fgfg.png" alt=""><figcaption></figcaption></figure>

</div>

<div>

<figure><img src="../../.gitbook/assets/ffgfgf.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/ghhh.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About** Podgrab **image we used.**

This is the official Podgrab image.

**Can I deploy my own** Podgrab **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going.

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, , media, entertainment

</details>
