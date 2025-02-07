---
description: >-
  Kavita is your high-speed digital library, offering quick access to a diverse
  range of file formats. Organize your books and manga with this sleek and
  user-friendly tool.
cover: ../../.gitbook/assets/Screenshot 2023-09-12 180617.png
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

# 🖥 Kavita Deployment

### <mark style="color:blue;">What's is kavita?</mark>

<mark style="color:orange;">**Introducing Kavita: Your Rocket-Powered Digital Library**</mark>

<mark style="color:orange;">In the vast universe of digital libraries, Kavita shines like a shooting star. This self-hosted wonder is not your average library—it's a high-speed, sleek, and versatile repository for a wide array of file formats.</mark>

🚀 **Lightning-Fast & Elegant** 🎩 Kavita is like the Flash of digital libraries, giving you supersonic access to your literary treasures. Its slick design isn't just eye candy; it's an intuitive guide to your reading world. With Kavita, you're always just a click away from your reading lists and collections.

📚 **A Haven for Bookworms & Manga Enthusiasts** 📖 Whether you're a bookworm diving into novels or a manga aficionado exploring epic worlds, Kavita welcomes you. It neatly organizes your manga, comics, and books in one place, each series properly labeled, creating a harmonious symphony of literary order.

⭐ **Ratings & Reviews at Your Fingertips** 📝 Kavita isn't just a library; it's a community. You can rate and review your favorite manga, sharing your thoughts with fellow enthusiasts. It's like having a book club that never sleeps.

🔍 **Swift Searches, Like Magic** 🔮 Kavita has a magic trick up its sleeve: lightning-fast search. As you start typing, your manga appears as if by sorcery. It's the closest thing to mind-reading for a digital library.

🔐 **User & Library Management, Simplified** 📊 Managing your library has never been easier. Kavita offers rich user-based roles, authentication, and library management—all from within the app. It's the command center for your literary kingdom.

In the realm of digital libraries, Kavita isn't just a star; it's a supernova. It's where speed, style, and substance converge, offering you a portal to explore the vast galaxies of literature. Discover Kavita, where your reading experience goes beyond the ordinary and reaches for the stars

### <mark style="color:blue;">**How It Works**</mark>

**Unlocking Kavita: Your Digital Library's Inner Workings**

Ever wondered how a digital library as swift and powerful as Kavita operates behind the scenes? Let's dive into the mechanics that make Kavita tick.

📥 **File Format Versatility** 🧩 Kavita embraces a wide array of file formats, making it the ideal haven for all your literary treasures. Whether it's an epic fantasy novel, a thrilling comic, or a captivating manga series, Kavita accommodates them all.

🏠 **Homepage Haven** 🏡 Your journey often begins at the homepage. Here, you can swiftly resume your reading adventures, access your meticulously curated reading lists, and peruse your collections. It's your literary command center.

📚 **Library Organization** 📂 Imagine having all your series neatly cataloged in one place, with each bearing its rightful name. Kavita does just that, ensuring your library is an oasis of order and accessibility.

⭐ **Community Spirit** 🤝 Kavita isn't just about reading; it's about connecting. Share your thoughts and opinions by rating and reviewing your favorite manga and books. It's a virtual book club, alive with vibrant discussions.

🔍 **Instant Search Magic** 🎩 Searching for your desired manga is like casting a spell. Start typing, and like magic, your manga appears before you. It's a testament to Kavita's commitment to swift access.

🔐 **User & Library Management** 📊 The heart of Kavita's functionality lies in its robust user management and library organization features. With user-based roles, authentication, and intuitive library management tools, Kavita offers control and order to your literary universe.

Behind its elegant interface, Kavita is a sophisticated piece of technology designed to make your literary journey seamless and enjoyable. It's a digital realm where your favorite stories come to life, and where every page turned feels like an adventure. Welcome to Kavita, where the magic of literature meets the power of technology.

### <mark style="color:blue;">Steps And Procedure</mark>

&#x20;<mark style="background-color:purple;">**This deployment utilizes the official kavita Docker image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find  [kizaing/kavita](https://hub.docker.com/r/kizaing/kavita)  application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the  kavita  application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the   kavita webpage and explore its content.

By following these straightforward steps, you'll have successfully deployed the  kavita application and gained access to its features through a seamless and user-friendly process.



### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------- |
| [kavita ](https://hub.docker.com/r/kizaing/kavita) <mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                                |
| ------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: kavita (you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">5000</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

| Install with Default                                                                                                                                        | Advanced                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">(select this if you want install with default settings if don't have environment value and working directory)</mark> | <mark style="background-color:yellow;">(select this if you want to go with advanced settings, where you select you own environment value and working directory)</mark> |

If you choose Advanced option:

| ENV VARIABLE                                                            |
| ----------------------------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> |

| WORKING DIR                                                                                                  |
| ------------------------------------------------------------------------------------------------------------ |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p>                      |
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                                      |
| <p></p><pre><code>-v /your/manga/directory:/manga \
-v /kavita/data/directory:/kavita/config \
</code></pre> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to kavita Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> Kavita
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name:  Kavita
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `5000`
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
           -v /your/manga/directory:/manga \
           -v /kavita/data/directory:/kavita/config \
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an  Kavita instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/cvcb (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/vbfd (1).png" alt=""><figcaption></figcaption></figure>

</div>

<div>

<figure><img src="../../.gitbook/assets/dfdfd (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/ddfdfdf (1).png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About** Kavita **image we used.**

This is the official  Kavita image.

**Can I deploy my own** Kavita **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, Kavita

</details>
