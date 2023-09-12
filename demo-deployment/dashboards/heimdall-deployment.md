---
cover: >-
  ../../.gitbook/assets/68747470733a2f2f692e696d6775722e636f6d2f697556387733792e706e67.png
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

# 🖥 Heimdall Deployment

### <mark style="color:blue;">What's is heimdall?</mark>

**Heimdall Dashboard: Where Web Apps Find Harmony**

Tired of juggling countless tabs and bookmarks for your favorite web applications? Meet Heimdall Application Dashboard, your one-stop solution for taming the chaos and bringing order to your digital life.

**1. Unified Web App Haven:**

* _All Roads Lead to Heimdall_: Say goodbye to tab overload! Heimdall Dashboard consolidates all your web applications, tools, and services into a single, elegantly organized space.

**2. Customization Galore:**

* _Tailor Your Experience_: Heimdall empowers you to shape your dashboard as you see fit. Add links to web applications, search engines, or even set it as your browser's start page. It's your digital canvas—paint it your way.

**3. Visual Pleasure:**

* _Elegance Meets Functionality_: Heimdall doesn't just organize; it delights the eye. Discover visually appealing apps that make managing your digital realm a joyous experience.

**4. Apps API Magic:**

* _Your Access Pass_: Dive into an array of enhanced apps, foundation apps, and generic items via Heimdall's apps API. It's your express route to swift access for your go-to web applications and services.

**5. Simplified Streamlining:**

* _Time-Saving Brilliance_: Heimdall is your digital efficiency partner. It ensures you spend less time searching for tools and more time using them. It's your personalized launchpad to the digital world.

**6. Beyond Apps Alone:**

* _Freedom to Choose_: Heimdall isn't confined to apps. It's your canvas for organizing anything—web apps, resources, or even personal shortcuts. Your preferences set the limits, and they're practically limitless.

In essence, Heimdall Application Dashboard is where chaos meets order, where scattered web applications find unity, and where customization reigns supreme. With Heimdall, your digital life becomes an elegantly orchestrated symphony, with all your favorite apps and tools harmoniously brought together. Say hello to simplicity, visual delight, and efficiency, and make Heimdall your portal to a more organized and enjoyable online experience

### <mark style="color:blue;">**How It Works:**</mark>

**Navigating the Heimdall Dashboard: A Symphony of Digital Organization**

_The Heimdall Application Dashboard_ functions as your digital conductor, orchestrating a seamless symphony of web applications, services, and tools. Here's how this harmonious platform works its magic:

**1. Entry to Elegance:**

* **Unified Hub:** Upon launching Heimdall, you're greeted with a unified hub that corrals all your digital essentials into one visually pleasing space.

**2. Personalized Precision:**

* **Tailor-Made Dashboard:** The power is in your hands. Customize your dashboard by adding links to web apps, search engines, or even adopting it as your browser's start page. It's a canvas where you dictate the composition.

**3. Aesthetic Appeal:**

* **Visual Treat:** Heimdall isn't just functional; it's aesthetically delightful. Explore visually captivating apps that transform mundane management into a pleasurable experience.

**4. API Access:**

* **App Exploration:** Dive into the world of enhanced apps, foundation apps, and generic items through Heimdall's apps API. This is your express lane to instant access for your most-visited web applications and services.

**5. Streamlined Efficiency:**

* **Time-Saving Brilliance:** Heimdall is your efficiency companion. Spend less time hunting for tools and more time utilizing them. It's your personalized portal to the digital universe.

**6. Boundless Freedom:**

* **No Limits:** Heimdall extends beyond applications. It's your canvas for organizing anything—web apps, resources, or even personal shortcuts. Your preferences set the boundaries, and those boundaries are nearly infinite.

In essence, _Heimdall Application Dashboard_ takes the chaos of scattered web applications and transforms it into a symphony of organization. It's where customization reigns supreme, your digital life finds unity, and the mundane becomes a visual delight. Embrace simplicity, efficiency, and a touch of elegance with Heimdall, your gateway to a more organized and enjoyable online journey

### <mark style="color:blue;">Steps And Procedure</mark>

&#x20;<mark style="background-color:purple;">**This deployment utilizes the official Heimdall Docker image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find the l[inuxserver/heimdall](https://hub.docker.com/r/linuxserver/heimdall) application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the _Heimdall_ application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the  _Heimdall_ webpage and explore its content.

By following these straightforward steps, you'll have successfully deployed the _Heimdall_ application and gained access to its features through a seamless and user-friendly process.



### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                 |
| -------------------------------------------------------------------------------------------------------------------------------------------- |
| [heimdall](https://hub.docker.com/r/linuxserver/heimdall) <mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                                 |
| -------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: heimdall(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">80</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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

<mark style="color:purple;">**Step-by-Step Guide to heimdall Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name: heimdall</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: heimdall
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
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an _Heimdall_ instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-11 180032.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-11 180102.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-11 180203.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-11 180321.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-11 180254.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About** _Heimdall_ **image we used.**

This is the official _Heimdall_ image.

**Can I deploy my own** _Heimdall_ **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
