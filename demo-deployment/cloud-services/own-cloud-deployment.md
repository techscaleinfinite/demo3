---
description: >-
  OwnCloud, the game-changer in data management, puts you in control of your own
  cloud storage. Keep your data securely within your reach with this robust and
  open-source platform.
cover: ../../.gitbook/assets/ownCloud-Trademark.png
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

# ☁ Own Cloud Deployment

### <mark style="color:blue;">What's  OWNCLOUD?</mark>

<mark style="color:orange;">OwnCloud is a game-changer in the realm of data management, offering a comprehensive open-source platform that puts you in the driver's seat when it comes to your data. Here's a closer look:</mark>

**1. **<mark style="color:orange;">**Data Ownership:**</mark>

* OwnCloud places the power of data ownership squarely in your hands. It allows you to establish and manage your very own cloud storage system on your servers. This means that your data remains securely within your control, residing exactly where you want it – under your own roof.

<mark style="color:green;">**2. Fortified Data Access:**</mark>

* Security is paramount, and OwnCloud takes it seriously. It provides robust and secure access to your files, ensuring that only authorized individuals can view and share them. It functions as a digital fortress, safeguarding your digital assets with top-notch protection.

<mark style="color:blue;">**3. Seamless Sharing and Collaboration:**</mark>

* Need to collaborate with colleagues or partners? OwnCloud simplifies the process. It offers effortless file sharing and collaboration tools, akin to having your own exclusive virtual conference room in the cloud. This means you and your team can collaborate seamlessly, regardless of your geographical locations.

In an era where data privacy and control are of utmost importance, OwnCloud stands as a beacon of empowerment. It offers you the means to exercise complete control over your data, guarantees its safety, and facilitates effortless collaboration. Whether you're an individual or a large organization, OwnCloud is your steadfast ally in the pursuit of secure, accessible, and well-managed data. It's your key to data sovereignty in an increasingly data-centric world.

### <mark style="color:blue;">**How It Work:**</mark>

\
<mark style="color:orange;">Sync and Share Files: With ownCloud at your disposal, you gain the incredible ability to synchronize files and folders seamlessly across all your devices. Whether it's your trusted computer, your favorite smartphone, or a reliable tablet, ownCloud acts like your personal butler, ensuring you have your digital belongings with you wherever you go. This promotes effortless collaboration and enhances your productivity, much like having a faithful companion by your side.</mark>

Self-Hosted Solution: Say farewell to the era of relying on third-party cloud storage providers. ownCloud grants you the power to keep your data exactly where you want it – on your own servers or infrastructure. It's akin to having a digital fortress, with you as the guardian of your privacy and data security, ensuring that your digital assets remain under your watchful eye.

<mark style="color:yellow;">User-Friendly Web Interface:</mark> Navigating ownCloud is a breeze, thanks to its intuitive web interface. It resembles a traditional file manager, making it a cinch to upload, organize, and manage your files. It's like having an old friend assisting you in organizing your digital life, simplifying tasks that might otherwise seem daunting.

<mark style="color:yellow;">Access Control and Sharing:</mark> Sharing files and folders has never been easier. ownCloud streamlines this process, allowing you to set specific permissions for those who can view and edit your content. It's akin to being the conductor of a digital orchestra, providing you with the tools to collaborate seamlessly and harmoniously.

S<mark style="color:blue;">ecurity and Encryption:</mark> At ownCloud, your data's security takes precedence. It ensures your files are locked with encryption both in storage and during transit, keeping them safe from prying eyes. Moreover, you retain the ability to manage your encryption keys, affording you an additional layer of control over your precious data.

<mark style="color:yellow;">Integration with External Memory:</mark> ownCloud is a true team player, capable of syncing with various storage sources such as FTP, Amazon S3, and Google Drive. This allows you to centralize all your data neatly under one roof, simplifying data management.

<mark style="color:green;">Application Ecosystem:</mark> Consider ownCloud your personal application playground. It offers a rich assortment of apps and plugins that can enhance your cloud hosting experience. From calendaring to document editing, you have the freedom to tailor your ownCloud to suit your unique requirements.

_Collaborative Editing: When the need arises for collaborative document editing, ownCloud has you covered. It fully supports real-time collaborative editing, enabling multiple individuals to work on the same document simultaneously. This eliminates the need for cumbersome email attachments and fosters efficient teamwork._

<mark style="color:green;">File Versioning:</mark> Don't fret about keeping track of file versions; ownCloud handles it for you. It maintains a comprehensive record, allowing you to roll back to previous versions whenever necessary. It's akin to having a time machine at your disposal, ensuring your documents are always in order.

<mark style="color:red;">Mobile Application:</mark> For those on the move, ownCloud stands ready to assist. With mobile apps designed for Android and iOS, you can access and manage your files from virtually anywhere, putting the power of ownCloud in the palm of your hand.

<mark style="color:purple;">Extensible and Customizable:</mark> If you're the DIY type, ownCloud's open-source nature invites you to explore and expand its functionality as you see fit. You have the creative freedom to customize and extend ownCloud to meet your ever-evolving needs.

In a world where data control and collaboration are of paramount importance, ownCloud emerges as your faithful companion – a user-friendly, secure, and adaptable platform ready to cater to your ever-changing digital requirements. It's akin to having a Swiss Army knife for your data, always at the ready to tackle any task with finesse.

### <mark style="color:blue;">Steps And Procedure</mark>

<mark style="background-color:green;">**This deployment utilizes the official OWNCLOUD Docker image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find the OWN CLOUD application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the OWNCLOUD application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the OWNCLOUD webpage and explore its content.

By following these straightforward steps, you'll have successfully deployed the OWNCLOUD application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                                          |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<mark style="color:orange;">`owncload`</mark>](https://hub.docker.com/\_/owncloud)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                                  |
| --------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: OWNCLOUD1(you can put any name)</mark> |

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
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                 |
| /var/www/html                                                                           |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to OWNCLOUD Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`OWNCLOUD`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `owncloud`
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
       * <mark style="color:red;">Here use ( use the path after   " :"  )</mark>
       * /var/www/html
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an OWNCLOUD instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 164951.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 164926.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About owncloud image we used.**

This is the official owncloud image.

**Can I deploy my own owncloud image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, own cloud

</details>
