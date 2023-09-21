---
cover: ../../.gitbook/assets/rfgr.png
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

# 💹 Octobot Deployment

### <mark style="color:blue;">What's  octobot?</mark>

<mark style="color:orange;">**OctoBot: Where Crypto Trading Meets Simplicity and Profitability**</mark>

<mark style="color:orange;">In the complex world of cryptocurrency trading, OctoBot emerges as a game-changer, combining power, simplicity, and profitability. Let's dive into the heart of this innovative open-source cryptocurrency trading robot:</mark>

**1. Versatile Trading Strategies:**

* **Copy from OctoBot Cloud:** Soon, you'll have the option to seamlessly adopt trading strategies from the OctoBot Cloud.
* **Customization:** Modify and enhance existing strategies to suit your preferences.
* **Create Your Strategy:** Ambitious traders can craft and optimize their trading strategies with OctoBot Pro.

**2. User-Centric Approach:**

* **Time Efficiency:** OctoBot is designed for individuals with busy lives who want the best returns on their investments. Say goodbye to complexity and time-consuming trading.

**3. Inclusivity in Trading:**

* **No Trading Pro Required:** Unlike many trading tools built for professionals, OctoBot welcomes traders of all levels.
* **Community-Powered:** OctoBot Cloud thrives on strategies contributed by the community, making it a win-win for everyone. Share your successful strategies and earn more.

**4. Strategy Testing and Flexibility:**

* **Simulation Ready:** Test any strategy rigorously using historical data or live simulations.
* **No Limits:** Whether you're just starting or an expert trader, OctoBot offers limitless testing possibilities.

**5. Transparency and Evolution:**

* **Verifiable Robot:** OctoBot is transparent and open-source, ensuring you can trust its functionality.
* **Continuous Improvement:** It has been tried and tested since its inception in 2018, with the potential for ongoing improvements.

In essence, OctoBot empowers crypto-investors to harness the full potential of their investments. It's a platform where complexity is tamed, and profitability is within reach for traders of all backgrounds. With OctoBot, you're not just trading; you're trading smarter. 🤖💹🚀



### <mark style="color:blue;">**How It Works:**</mark>

<mark style="color:orange;">**OctoBot in Action: Unleashing Crypto Trading Potential**</mark>

<mark style="color:orange;">So, you're eager to explore how OctoBot works its magic in the world of cryptocurrency trading? Let's take a closer look at the inner workings of this innovative trading companion:</mark>

**1. Strategy Selection:**

* Begin by selecting your preferred trading strategy. You have options:
  * **Copy from OctoBot Cloud:** Soon, you'll access a library of proven strategies.
  * **Customization:** Modify existing strategies to align with your goals.
  * **Craft Your Strategy:** Ambitious traders can design and fine-tune strategies using OctoBot Pro.

**2. Efficient Automation:**

* Once your strategy is in place, OctoBot takes over the heavy lifting. It autonomously executes trades based on your chosen approach.

**3. Community Collaboration:**

* OctoBot thrives on collective wisdom. The OctoBot Cloud is fueled by strategies contributed by fellow traders. Share your winning strategies, and you'll reap the rewards.

**4. Rigorous Testing:**

* Curious about how your chosen strategy will perform? OctoBot enables comprehensive testing.
* Use historical data or engage in live simulations to refine your strategy further.

**5. Accessibility for All:**

* OctoBot breaks down barriers. It's designed for both novice and seasoned traders.
* No need to be a trading pro; OctoBot welcomes all skill levels.

**6. Open-Source Reliability:**

* Rest easy knowing that OctoBot is transparent and open-source. You can verify its operations and trust its integrity.

**7. Constant Evolution:**

* OctoBot isn't stagnant. It has been evolving since its inception in 2018, continually improving to meet the demands of the dynamic crypto landscape.

In essence, OctoBot streamlines cryptocurrency trading, making it accessible, efficient, and potentially lucrative for everyone. It's not just about trading; it's about trading smarter with OctoBot.

### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official octobot image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the  [drakkarsoftware/octobot](https://hub.docker.com/r/drakkarsoftware/octobot) application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the OctoBot  application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the OctoBot webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed the OctoBot application and gained access to its features through a seamless and user-friendly process.



### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                                                                                                                 |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [octobot ](https://hub.docker.com/r/drakkarsoftware/octobot)[<mark style="background-color:yellow;">👈(</mark>](https://hub.docker.com/r/linuxserver/firefox)<mark style="background-color:yellow;">click me,for the dockerhub image)</mark> |

| Application name                                                                |
| ------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: octobot(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">5001</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>



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
| <p></p><pre><code>/octobot/user
</code></pre>                                           |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to octobot Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name: octobot</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name:`octobot`
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `5001`
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
           /octobot/user
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an OctoBot   instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-11 124146.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-11 123331.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-11 123407.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-11 123751.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-11 124023.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-11 123941.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-11 123841.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.

### <mark style="color:blue;">FAQ</mark>

**About** OctoBot  **image we used.**

This is the official OctoBot   image.

**Can I deploy my own media** OctoBot  **with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
