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

# 🔒 Caddy Deploment

### <mark style="color:blue;">What's is caddy?</mark>

<mark style="color:orange;">Caddy is an open-source, modern web server that is designed to be simple, efficient, and secure. It aims to make the process of configuring and deploying web services easier by providing a user-friendly interface and automated features.</mark>

### <mark style="color:blue;">**How It Works:**</mark>

**Configuration:** Caddy's configuration is defined using a simple and human-readable Caddyfile.The Caddyfile allows you to specify how your web server should behave, including domain routing, TLS certificates, reverse proxying, and more.

**2. Automatic HTTPS:** One of Caddy's standout features is its automatic HTTPS provisioning. When you configure a domain in the Caddyfile, Caddy will automatically request and manage SSL/TLS certificates from Let's Encrypt to enable secure HTTPS connections for your websites. This process simplifies the setup of secure connections and eliminates the need for manual certificate management.

**3. Reverse Proxy:** Caddy can act as a reverse proxy, forwarding requests to other services based on domain or path matching. This makes it easy to host multiple services on a single server and route traffic to the appropriate backend applications.

**4. **<mark style="color:orange;">**Load Balancing**</mark>**:** Caddy supports load balancing across multiple backend servers, distributing incoming traffic to ensure high availability and improved performance.

**5. Rewrite and Redirection:** Caddy allows you to define URL rewrites and redirections, which can be useful for changing URLs or handling SEO-friendly redirects.

**6. Fast and Efficient:** Caddy is built with performance in mind. It uses modern web server technologies and is optimized to handle concurrent connections efficiently.

**7. Plugins and Middleware:** Caddy supports plugins and middleware that can extend its functionality. These can be used to add features like rate limiting, authentication, logging, and more.

**8. On-the-Fly Compression:** Caddy can automatically compress resources like CSS, JavaScript, and HTML on the fly,

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

| WORKING DIR                                                                             |
| --------------------------------------------------------------------------------------- |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p> |

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

**About plex image we used.**

This is the official plex image.

**Can I deploy my own plex image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!
