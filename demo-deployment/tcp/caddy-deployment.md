---
cover: ../../.gitbook/assets/caddy-open-graph.jpg
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

# 🔒 Caddy Deployment

### <mark style="color:blue;">What's is caddy?</mark>

### &#x20;<mark style="color:orange;">**Caddy: Where Simplicity Meets Security**</mark>

_<mark style="color:orange;">Introducing Caddy, the modern web server that's rewriting the script on simplicity, efficiency, and security. Here's the backstage pass:</mark>_

**A Web Server Reimagined:** Caddy isn't your typical web server; it's the avant-garde of the web hosting world. It's designed to break down complexity and hand you simplicity on a silver platter.

**User-Friendly Sorcery:** Configuring and deploying web services becomes as easy as waving a wand with Caddy. Say goodbye to the labyrinth of configuration files; Caddy offers a user-friendly interface that feels like magic.

**Efficiency Unleashed:** Caddy doesn't waste time. It's a well-oiled machine, delivering web content with finesse and speed. When it serves, it does so swiftly and efficiently.

**Guardian of Security:** Security isn't a feature; it's Caddy's mantra. It's engineered with layers of protection, ensuring that your web services stay safe and sound.

**Automation at Your Service:** Caddy automates the tedious tasks, so you can focus on the grand performance. It's the assistant that takes care of the nitty-gritty details.

_With Caddy, the web server experience is like a finely orchestrated symphony – harmonious, efficient, and utterly secure._

### <mark style="color:blue;">**How It Works**</mark>

<mark style="color:orange;">**Caddy's Feature Ensemble: Unveiled**</mark>

_<mark style="color:orange;">Caddy is a powerhouse of features that turn web server management into a breeze. Take a tour of its remarkable capabilities:</mark>_

**1. Configuration Simplified:** With Caddy, complex configurations are a thing of the past. Its Caddyfile speaks human, making it effortless to define how your web server should behave. No more deciphering cryptic code.

**2. HTTPS Made Effortless:** Caddy steals the show with its automatic HTTPS wizardry. When you set up a domain in the Caddyfile, it works its magic by summoning SSL/TLS certificates from Let's Encrypt. Secure connections? Consider it done – no manual certificate juggling required.

**3. Master of Reverse Proxy:** Caddy effortlessly moonlights as a reverse proxy, deftly rerouting requests to other services based on domain or path cues. Hosting multiple services on one server? Caddy's got your back, ensuring each request reaches its intended destination.

**4. Load Balancing Virtuoso:** For Caddy, load balancing is a walk in the park. It gracefully balances the incoming traffic across multiple backend servers, orchestrating high availability and turbocharged performance.

**5. Rewrite and Redirect Maven:** Need to tweak URLs or craft SEO-friendly redirects? Caddy's got you covered. It allows you to redefine URLs and perform elegant redirections – a boon for SEO strategists.

**6. Speed Demon:** Caddy doesn't believe in slowdowns. It's designed for speed, leveraging cutting-edge web server technologies to handle multiple connections with finesse.

**7. Plugins and Middleware Galore:** Caddy's versatility shines through its support for plugins and middleware. Whether it's rate limiting, authentication, or advanced logging, Caddy has the tools to elevate your web service.

**8. Compression On-the-Fly:** Caddy doesn't just serve; it optimizes. Automatically compressing resources like CSS, JavaScript, and HTML on the fly, it ensures your web content arrives in style – fast and efficient.

_Caddy – where power meets simplicity, and features take center stage._

### <mark style="color:blue;">Steps And Procedure</mark>

&#x20; <mark style="background-color:purple;">**This deployment utilizes the official caddy image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find the cadd application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the Caddy application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the  Caddy webpage and explore its content.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                                  |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<mark style="color:orange;">caddy</mark>](https://hub.docker.com/\_/caddy)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                              |
| ----------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: caddy(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td>80</td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td></td></tr></tbody></table>

| Install with Default                                                                                                                                        | Advanced                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">(select this if you want install with default settings if don't have environment value and working directory)</mark> | <mark style="background-color:yellow;">(select this if you want to go with advanced settings, where you select you own environment value and working directory)</mark> |

If you choose Advanced option:

| ENV VARIABLE                                                            |
| ----------------------------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> |

| WORKING DIR                                                                                               |
| --------------------------------------------------------------------------------------------------------- |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p>                   |
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                                   |
| <p></p><pre class="language-console"><code class="lang-console">/usr/share/caddy/index.html
</code></pre> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to caddy Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name: caddy</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: caddy
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: http
   * Port: 80
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

           ```console
           /usr/share/caddy/index.html
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an HOMER instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 162704.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 162815.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About caddy image we used.**

This is the official caddy image.

**Can I deploy my own caddy image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!