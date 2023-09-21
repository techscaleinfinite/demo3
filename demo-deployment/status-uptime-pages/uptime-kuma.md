---
cover: ../../.gitbook/assets/f21b61f5-693a-4925-9f1f-fea237ade223.png
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

# 📊 uptime kuma

### <mark style="color:blue;">What's  Uptime Kuma?</mark>

🕐 **Keeping Time with Uptime Kuma** 🕐

Imagine having a trusty companion, always on the lookout, tirelessly monitoring your websites, APIs, and services. Well, that's precisely what **Uptime Kuma** does, but with a little extra charm.

**Your Digital Sentry**&#x20;

Think of Uptime Kuma as your digital sentry, standing guard over your online empire. It's on a mission to make sure your websites, APIs, and services are always on their best behavior. Whenever they decide to take a coffee break (a.k.a. downtime), Uptime Kuma is there to give them a friendly nudge.

**Swift Response Times**&#x20;

Not only does Uptime Kuma keep an eagle eye on the availability of your digital assets, but it also tracks how fast they respond to requests. It's like having a stopwatch in the digital Olympics, ensuring that your services are always in tip-top shape.

📈 **Data Whisperer** 📈

Uptime Kuma is more than just a digital watchdog; it's also a data whisperer. It collects precious information about your applications' uptime and downtime, and it presents it to you in beautiful, informative graphs. It's like turning raw data into a symphony of insights.

**User-Friendly and Open-Source**&#x20;

And here's the kicker: Uptime Kuma is not only incredibly useful but also user-friendly. You don't need to be a tech genius to make sense of it. Plus, it's open-source, which means it's a labor of love from a community of tech enthusiasts.

So, with Uptime Kuma in your corner, your digital realm can be as reliable as Big Ben and as speedy as Usain Bolt. It's your trusty sidekick in the ever-watchful world of online monitoring!

### <mark style="color:blue;">**How It Works:**</mark>

🛠️ **The Magic Behind Uptime Kuma** 🛠️

Have you ever wondered what makes **Uptime Kuma** tick? How does it do its thing without breaking a digital sweat? Well, let's pull back the curtain and see the gears turning in this digital symphony.

🕵️‍♂️ **The Digital Detective** 🕵️‍♂️

At its core, Uptime Kuma is your very own digital detective, investigating the online world on your behalf. It's programmed to be inquisitive, scanning websites, APIs, and services to ensure they're all playing nice. When something seems amiss, Uptime Kuma's alarm bells start ringing.

🏁 **The Stopwatch Master** 🏁

Response times are Uptime Kuma's playground. It's like a stopwatch master, keeping tabs on how quickly your applications respond to requests. The faster, the better! It's a bit like watching a race, but with data packets sprinting to the finish line.

📊 **The Data Whisperer's Tale** 📊

Now, here's where the magic happens. Uptime Kuma collects data like a seasoned explorer, venturing through the vast wilderness of the internet. But instead of a compass, it uses graphs and charts to map its discoveries. These visualizations are your window into the uptime and downtime of your digital assets.

👩‍💻 **User-Friendly and Open to All** 👨‍💻

Uptime Kuma is built with simplicity in mind. You don't need a Ph.D. in tech jargon to understand it. It's designed to be as approachable as your favorite smartphone app. And being open-source, it's a product of passion and collaboration from tech enthusiasts worldwide.

So, there you have it – Uptime Kuma demystified! It's not just a tool; it's your digital guardian, your timekeeper, and your data whisperer, all rolled into one. With Uptime Kuma, your online empire stays strong and responsive, just as it should. 🌐🔍📈\


### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official UPTIMEKUMA Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the [louislam/uptime-kuma](https://hub.docker.com/r/louislam/uptime-kuma) application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the  Uptime Kuma application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the l Uptime Kuma webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed   Uptime Kuma application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                   |
| ---------------------------------------------------------------------------------------------------------------------------------------------- |
| [uptime kuma](https://hub.docker.com/r/louislam/uptime-kuma)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                              |
| ----------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: KUMA1(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">3001</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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
| <p></p><pre class="language-bash"><code class="lang-bash">-v uptime-kuma:/app/data
</code></pre> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to UPTIME KUMA Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark><mark style="color:orange;">`UPTIME KUMA`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: uptime kuma
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `3001`
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

           ```bash
           -v uptime-kuma:/app/data
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an  Uptime Kuma instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/nnn.pngjbjfuyfuygu.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/lloooll.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/loloi.png" alt=""><figcaption></figcaption></figure>

</div>

<div>

<figure><img src="../../.gitbook/assets/poooi.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/tyt.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/oiuuu.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About**  uptime kuma **image we used.**

This is the official uptime kuma  image.

**Can I deploy my own** uptime kuma **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
