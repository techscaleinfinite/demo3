---
cover: ../../.gitbook/assets/original.png
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

# Mini game Deployment

### <mark style="color:blue;">What's  mini games?</mark>

This evolving game is like a playground for learning and experimenting with web technologies while diving into the world of multiplayer, high-speed, mobile gaming. It's an exciting journey to uncover the sweet spots and boundaries of what the web can do in this gaming space.

Imagine this game as a collection of parallel universes, where each player has their universe filled with unique physics and interactions. It's like having your own sandbox to play in. But what makes it even more thrilling is that these universes are all connected through magical portals, allowing players to team up and tackle challenges together.

If you're playing on a touch screen device, just a simple tap on your character makes them jump, bringing your actions to life with a gentle touch. For those with keyboards, the trusty arrow keys join the fun, offering an additional way to navigate this exciting world.

While this game is still in its early stages, there's a lot of focus on perfecting the animation system, handling player input seamlessly, and ensuring that the communication between the frontend (what you see) and the backend (where the magic happens) is as smooth as possible.

You can experience this adventure right now by visiting [https://mini-game.oliverlanz.ch](https://mini-game.oliverlanz.ch/). The real magic happens when you connect multiple devices simultaneously. So grab your friends, your smartphones, tablets, and laptops, and embark on this epic journey together. It's a world where the web transforms into a playground of endless possibilities. Give it a try, and let the gaming begin!

### <mark style="color:blue;">**How It Works:**</mark>

The inner workings of this fascinating game involve a combination of innovative concepts and web technologies. Let's take a closer look at how it all comes together:

**1. Parallel Universes:** In this game, the core concept revolves around the existence of parallel universes. Each player inhabits their distinct universe, complete with its set of rules, physics, and interactions. This design allows for a personalized gaming experience within a shared multiplayer environment.

**2. Interconnected Universes:** While players have their separate universes, they are all interconnected through mystical portals. These portals act as bridges between the parallel worlds, enabling players to collaborate and work together to achieve common objectives. This connectivity adds a layer of complexity and cooperation to the gameplay.

**3. User-Friendly Controls:** The game has been designed to cater to a wide range of devices. On touch screen devices, players can easily make their characters jump with a simple tap. For those using devices with keyboards, traditional arrow keys provide an alternative means of control. This versatility ensures that players can enjoy the game regardless of their preferred input method.

**4. Current Development Focus:** While the game is in its early stages of development, specific areas are receiving special attention. The animation system is being refined to provide smooth and visually appealing movements. Input handling mechanisms are being optimized to ensure responsive and intuitive controls. Additionally, the communication between the frontend (the visible part of the game) and the backend (the underlying logic) is being fine-tuned for seamless interaction.

**5. Interactive Exploration:** To experience this evolving game, you can visit [https://mini-game.oliverlanz.ch](https://mini-game.oliverlanz.ch/). The real magic happens when you connect multiple devices simultaneously. This interactive aspect allows you and your friends to embark on this journey together, exploring the boundaries of what web technologies can offer in the realm of multiplayer, high-FPS, mobile gaming.

In summary, this game is a captivating experiment that pushes the boundaries of web technologies in the context of multiplayer mobile gaming. It combines the concepts of parallel universes, interconnected gameplay, and versatile controls to create an engaging and evolving gaming experience. So, gather your friends and devices and dive into this unique web-based adventure

### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official mini game Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the [olilanz/mini-game](https://hub.docker.com/r/olilanz/mini-game)application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the minigame    application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the  minigame  webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed the minigame application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                                |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [ ](https://hub.docker.com/\_/varnish)[minigame](mini-game-deployment.md)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                             |
| ---------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: mini(you can put any name)</mark> |

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

<mark style="color:purple;">**Step-by-Step Guide to MINI GAME Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`minigame`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `MINIGAME`
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

By following these steps, you can effortlessly deploy an minigame instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-06 161831.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-06 162153.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About** minigame **image we used.**

This is the official minigame image.

**Can I deploy my own** minigame **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
