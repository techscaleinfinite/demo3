---
cover: ../../.gitbook/assets/y70e9tix7a_._sablona-web-titulniObrazek.png
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

# 🖥 Node Red Deployment

### <mark style="color:blue;">What's node red?</mark>

<mark style="color:orange;">**Node-RED: Unleash Your Creativity with the Ultimate Hardware and API Wiring Tool**</mark>

<mark style="color:orange;">Ever felt the itch to connect the digital dots in exciting and unconventional ways? That's precisely where Node-RED steps in – your programming companion for orchestrating a symphony of hardware devices, APIs, and online services.</mark>

**1. Visual Wiring:** Picture this – a browser-based editor that lets you effortlessly wire together flows. It's like playing with digital Lego blocks. Choose from a vast palette of nodes and bring your imaginative flows to life.

**2. One-Click Deployment:** Turning your ideas into reality couldn't be simpler. With Node-RED, it's just a single click to deploy your meticulously crafted flows onto the runtime. Your creations spring to life instantly.

**3. Code Craftsmanship:** Feel the urge to dive into some JavaScript wizardry? Node-RED's editor boasts a rich text editor for crafting intricate JavaScript functions. Your code, your rules.

**4. Library of Wonders:** Ever stumbled upon a genius piece of code? Node-RED lets you save these nuggets in its built-in library. Functions, templates, or entire flows – it's your treasure chest of digital gems.

**5. JSON Magic:** Behind the scenes, Node-RED's wizardry stores your flows as JSON. Import, export, and share your creations effortlessly with JSON's flexibility.

**6. Flow Showcase:** Feeling generous? Share your finest flows with the world through Node-RED's online flow library. It's your stage to shine and inspire others.

Node-RED isn't just a tool; it's your canvas for digital artistry. Whether you're weaving the threads of IoT devices, orchestrating APIs, or unraveling the mysteries of online services, Node-RED is your trusted ally.

So, seize your browser-based brush and start painting the future of connectivity with Node-RED. Your imagination is the limit, and the digital world is your canvas. Create, connect, and innovate!

### <mark style="color:blue;">**How It Works**</mark>

**1. Visual Wiring –** Think of Node-RED as your digital playground. It provides a browser-based editor that's as intuitive as connecting building blocks. You choose nodes from a diverse palette and effortlessly link them together. It's like painting a digital masterpiece, one stroke at a time.

**2. One-Click Deployment –** Now, imagine your creation is ready to come to life. With Node-RED, it's not a complex ritual. A single click, and your imaginative flows are deployed onto the runtime. It's like hitting the "Go" button on your digital rollercoaster.

**3. Code Craftsmanship –** For those moments when you're feeling particularly adventurous, Node-RED's editor includes a rich text editor for crafting JavaScript functions. It's your digital playground, where you're the coder and the conductor of this digital orchestra.

**4. Library of Wonders –** Ever come across a piece of code that's pure genius? Node-RED allows you to preserve these treasures in its built-in library. Whether it's a function, a template, or an entire flow, consider it your chest of digital wonders.

**5. JSON Magic –** Behind the scenes, Node-RED stores your creations as JSON. This format offers flexibility galore. Import, export, and share your flows effortlessly. It's like exchanging digital recipes with fellow chefs.

**6. Flow Showcase –** Feeling generous or simply proud of your creation? Node-RED's online flow library is your stage. Share your finest flows with the world. It's where innovation meets inspiration.

Node-RED isn't just a tool; it's your creative canvas for digital artistry. Whether you're orchestrating the symphony of IoT devices, weaving the threads of APIs, or exploring the vast world of online services, Node-RED is your trusty companion.

So, grab your digital brush, open the browser-based canvas, and start painting the future of connectivity with Node-RED. Your imagination sets the boundaries, and the digital world eagerly awaits your next masterpiece. Create, connect, and innovate!

### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official node red Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the [nodered/node-red](https://hub.docker.com/r/nodered/node-red/) application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the Node-RED application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the Node-RED  webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed the Node-RED application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                              |
| ----------------------------------------------------------------------------------------------------------------------------------------- |
| [node red ](https://hub.docker.com/r/nodered/node-red/)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                             |
| ---------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: node(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td>1880</td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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
| <p></p><pre><code>-v myNodeREDdata:/data
</code></pre>                                  |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to MEDIAWIKI Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`mediawiki`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `mediawiki`
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `1880`
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

           ```
           -v myNodeREDdata:/data
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an Node-RED instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-12 122450.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-12 122509.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-12 122747.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About media** Node-RED **we used.**

This is the official Node-RED image.

**Can I deploy my own media** Node-RED **with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
