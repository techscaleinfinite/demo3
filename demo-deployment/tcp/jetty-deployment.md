---
description: >-
  Jetty, also known as Eclipse Jetty, is your versatile open-source web server
  and servlet container. It's lightweight, scalable, and Java-based, making it a
  top choice for modern web applications.
cover: ../../.gitbook/assets/download (5).png
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

# 🖥 Jetty Deployment

### <mark style="color:blue;">What's  jetty?</mark>

J<mark style="color:orange;">etty, often referred to as Eclipse Jetty, is an open-source web server and servlet container. It is developed as part of the Eclipse Foundation's community-driven projects and is written in Java. Jetty is designed to be highly scalable, lightweight, and embeddable, making it a popular choice for a wide range of web-based applications and services. Here are some key aspects of Jetty:</mark>

1. **Web Server**: Jetty primarily functions as a web server, serving web content, static files, and handling HTTP requests. It supports various HTTP versions, including HTTP/1.1 and HTTP/2, making it suitable for modern web applications.
2. <mark style="color:red;">**Servlet Container**</mark><mark style="color:red;">:</mark> Jetty also serves as a servlet container, implementing the Java Servlet API. This means it can host Java servlets and JavaServer Pages (JSP), making it compatible with a wide range of Java-based web applications.
3. **Embedded Deployment**: One of Jetty's strengths is its ability to be embedded within other Java applications. Developers can include Jetty as a library and configure it programmatically. This is especially useful for microservices and embedded systems.
4. <mark style="color:purple;">**Scalability**</mark><mark style="color:purple;">:</mark> Jetty is known for its scalability. It can efficiently handle a large number of concurrent connections and requests, making it suitable for high-traffic websites and web services.
5. <mark style="color:red;">**Low Resource Usage**</mark>: Jetty is designed to be lightweight, with a small memory footprint. This makes it suitable for resource-constrained environments or scenarios where efficient resource usage is critical.
6. **Modular Architecture**: Jetty adopts a modular architecture, allowing users to include only the components they need. This reduces the overall footprint and helps maintain a minimal attack surface.
7. <mark style="color:orange;">**WebSocket Support**</mark><mark style="color:orange;">:</mark> Jetty provides built-in support for WebSocket, enabling real-time bidirectional communication between clients and servers. This is essential for applications that require instant data updates.

### <mark style="color:blue;">**How It Works**</mark>

<mark style="color:orange;">Jetty works as a web server and servlet container to handle incoming HTTP requests, serve web content, and execute Java servlets and JavaServer Pages (JSP). Here's a simplified overview of how Jetty works:</mark>

1. **Initialization**: Jetty is typically embedded within a Java application as a library. When the application starts, Jetty is initialized programmatically, and the necessary configurations are set up.
2. <mark style="color:orange;">**HTTP Server**</mark><mark style="color:orange;">:</mark> Jetty listens on a specified network port (e.g., port 8080) for incoming HTTP requests. It can also be configured to support secure connections via HTTPS.
3. **Request Handling**: When an HTTP request (e.g., a web page request or API call) is received on the configured port, Jetty's request handling mechanism takes over.
4. <mark style="color:green;">**Servlet Container**</mark><mark style="color:green;">:</mark> If the request is destined for a Java servlet or JSP, Jetty's servlet container component processes it. The servlet container manages the servlet lifecycle, including instantiation, initialization, and execution of the servlet's `doGet()` or `doPost()` methods.
5. <mark style="color:green;">**Static Content**</mark><mark style="color:green;">:</mark> If the request is for static content (e.g., HTML, CSS, JavaScript files), Jetty serves these files directly from the configured directory without involving the servlet container. This improves performance for static assets.
6. **Request Routing**: Jetty has a URL mapping mechanism that directs incoming requests to the appropriate servlet or resource based on the URL path. This routing ensures that each request is processed by the correct component.

### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official jetty Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the <mark style="color:orange;">jetty</mark> application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the jetty application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the jetty webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed the Nginx application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                 |
| ---------------------------------------------------------------------------------------------------------------------------- |
| [`jetty`](https://hub.docker.com/\_/jetty)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                              |
| ----------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: jetty(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">80/8080/443/8443</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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
| /usr/local/jetty/webapps                                                                |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to jetty Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`jetty`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `jetty`
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
       * <mark style="color:red;">Here use ( use the path after   " :"  )</mark>
       * /usr/local/jetty/webapps
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an jetty instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<figure><img src="../../.gitbook/assets/Screenshot 2023-09-01 160728 (1).png" alt=""><figcaption></figcaption></figure>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About httpd image we used.**

This is the official httpd image.

**Can I deploy my own httpd image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, jetty

</details>
