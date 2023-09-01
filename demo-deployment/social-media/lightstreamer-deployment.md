---
cover: ../../.gitbook/assets/download (1).jpg
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

# LightStreamer Deployment

### <mark style="color:blue;">What's LightStreamer?</mark>

Lightstreamer is a real-time messaging server that is optimized for the Internet. It's designed to facilitate real-time data streaming and messaging, making it a valuable tool for various applications and industries. The Docker Official Image for Lightstreamer simplifies the deployment of this messaging server, allowing users to easily set up and run Lightstreamer in a containerized environment.

Here are some key points about Lightstreamer and its Docker Official Image:

1. **Real-Time Messaging:** Lightstreamer is built to handle real-time messaging and data streaming. It can efficiently transmit data in real-time over the Internet, making it ideal for applications that require instant data updates.
2. **Optimized for the Internet:** Lightstreamer is optimized to work well in Internet-based scenarios, where low latency and efficient data transmission are crucial. It's commonly used in financial services, gaming, e-commerce, and other industries where real-time data is essential.
3. **Docker Official Image:** The Docker Official Image for Lightstreamer is a pre-packaged containerized version of the Lightstreamer server. This image is available on Docker Hub, making it easy for users to deploy Lightstreamer in a containerized environment.
4. **Containerization Benefits:** Using Docker containers offers benefits such as easy deployment, scalability, and isolation. With the Docker Official Image, users can quickly set up and run Lightstreamer instances on various platforms that support Docker.
5. **Scalability:** Lightstreamer can be deployed in a scalable manner, allowing organizations to handle increasing amounts of real-time data and users as their needs grow. Docker's container orchestration tools, such as Kubernetes, can be used to manage and scale Lightstreamer containers effectively.
6. **Use Cases:** Lightstreamer is used in a wide range of applications, including financial trading platforms, online gaming, live sports scoring, chat applications, and more. Any scenario that requires real-time data delivery can benefit from Lightstreamer's capabilities.
7. **Community and Support:** With a substantial user base and community support, Lightstreamer users can access resources, documentation, and forums for assistance and best practices.

In summary, Lightstreamer, when deployed using the Docker Official Image, provides a convenient way to set up a real-time messaging server optimized for the Internet. Its versatility and efficiency make it a valuable tool for applications that depend on real-time data updates and communication.

### <mark style="color:blue;">**How It Works:**</mark>

1. **Client-Server Architecture:** Lightstreamer follows a client-server architecture. Clients can be web browsers, mobile apps, or any software that needs real-time data updates. The server runs Lightstreamer and manages the communication with connected clients.
2. **Connection Establishment:** Clients initiate a connection to the Lightstreamer server using standard protocols such as HTTP, HTTPS, or WebSockets. The connection can be secured with encryption to ensure data privacy and security.
3. **Subscription Model:** Clients subscribe to specific data feeds or "items" that they are interested in. These items can represent various types of data, such as stock prices, sports scores, chat messages, or any real-time information.
4. **Data Providers:** Lightstreamer connects to data sources or providers, which can be databases, backend systems, or external data feeds. These providers are responsible for supplying the actual data that clients have subscribed to.
5. **Real-Time Data Push:** As soon as new data is available or changes occur in the subscribed items, the Lightstreamer server pushes these updates to the connected clients. This push mechanism ensures that clients receive data in real-time without the need for continuous polling.
6. **Bidirectional Communication:** Lightstreamer allows bidirectional communication between clients and the server. Clients can also send data or commands to the server, enabling interactive features like live chat, gaming moves, or trading orders.
7. **Scalability:** Lightstreamer is designed for scalability. To handle a large number of clients and data feeds, you can deploy multiple instances of Lightstreamer servers and load balance incoming connections. This ensures that the system can scale horizontally to meet increased demand.
8. **Failover and High Availability:** Lightstreamer supports failover and high availability configurations to ensure uninterrupted service. If one server instance fails, clients can seamlessly reconnect to another available server.
9. **Integration:** Lightstreamer can be integrated with various programming languages, platforms, and frameworks. It provides SDKs and libraries for popular languages like JavaScript, Java, .NET, and more, making it adaptable to different development environments.
10. **Use Cases:** Lightstreamer is used in diverse applications, including financial trading platforms for real-time stock data, online gaming for instant game updates, live sports apps for score updates, and collaborative tools for real-time document editing and chat.

### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official lightstream Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the lightstreamer application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the lightstreamer application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the lightstreamer webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed the lightstreamer application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                 |
| -------------------------------------------------------------------------------------------------------------------------------------------- |
| [`lightstreamer`](https://hub.docker.com/\_/lightstreamer)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                              |
| ----------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: light(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">8080</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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

<mark style="color:purple;">**Step-by-Step Guide to lightstreamer Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`lightstreamer`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `lightstreamer`
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
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an lightstreamer instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-01 183556.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-01 183459.png" alt=""><figcaption></figcaption></figure>

</div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-01 183437.png" alt=""><figcaption></figcaption></figure>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About**  lightstreamer **image we used.**

This is the officia lightstreamer image.

**Can I deploy my own** lightstreamer **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
