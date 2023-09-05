---
cover: ../../.gitbook/assets/ownCloud-Trademark.png
coverY: 0
---

# ☁ Own Cloud Deployment

### <mark style="color:blue;">What's  OWNCLOUD?</mark>

"OwnCloud" is a game-changer in the world of data management. It's an open-source software platform that doesn't just offer file synchronization and sharing services; it empowers individuals and organizations to take control of their data.

Here's the lowdown:

<mark style="color:orange;">**Data Ownership:**</mark> OwnCloud gives you the keys to the kingdom. It lets you set up your very own cloud storage solution on your servers. This means you're the captain of your data ship, and it stays right where you want it—under your roof.

**Secure File Access:** With OwnCloud, you can sleep soundly knowing your data is safe and sound. It provides secure access to your files, making sure only the right people can see and share them. It's like having a high-tech vault for your digital treasures.

<mark style="color:orange;">**Sharing Made Easy:**</mark> Need to collaborate? OwnCloud makes it a breeze. You can share files and collaborate with others seamlessly. It's like having your own private conference room in the cloud, where you and your team can work together, no matter where you are.

In a world where data privacy and control are paramount, OwnCloud is the champion. It's your ticket to data freedom, security, and collaboration—all in one open-source package. So, whether you're an individual or a big organization, OwnCloud is your ally in the quest for secure, accessible, and manageable data. 🌐🔐📂

### <mark style="color:blue;">**How It Work:**</mark>

1. <mark style="color:orange;">**Sync and share files:**</mark> With ownCloud, you have the ability to synchronize files and folders across all your devices, whether it's your trusted computer, popular smartphone, or trusted tablet. This is like having your own butler that ensures you take your belongings with you wherever you go, promoting seamless collaboration and productivity.
2. **Self-hosted solution**: Say goodbye to third-party cloud storage providers. With ownCloud, your data is where you want it: on your own servers or infrastructure. It's like having your own digital fortress where you are the guardian of your privacy and data security.
3. <mark style="color:orange;">**User-friendly web interface:**</mark> Navigating ownCloud is easy thanks to its user-friendly web interface. It looks like a traditional file manager, making it easy to upload, organize, and manage your files. It's like an old friend helping you organize your digital life.
4. **Access control and sharing**: Share files and folders? Nothing. ownCloud makes it easy to do this. You can set specific permissions for who can view and edit content. It's like being the conductor of a digital orchestra, allowing you to collaborate seamlessly.
5. **Security and encryption:** The security of your data is paramount to ownCloud. It locks your files with encryption in storage and in transit, away from prying eyes. Plus, you can manage your encryption keys, giving you an extra layer of control.
6. **Integration with external memory**: ownCloud is a team player. It can sync with other storage sources like FTP, Amazon S3, and Google Drive, helping you centralize all your data under one roof.
7. **Application ecosystem:** Think of ownCloud as your application playground. It offers a wealth of apps and plugins that enhance your cloud hosting experience. From calendaring to document editing, you can customize your own Cloud to fit your needs.
8. **Collaborative editing**: Need to work on documents together? ownCloud is here for you. It supports real-time collaborative editing, so multiple people can edit the same document at the same time. No more exchanging email attachments!
9. File version: Don't worry about file versions. ownCloud keeps the record for you, allowing you to roll back to previous versions if needed. It's like having a time machine for your documents.
10. **Mobile Application**: When you're on the go, ownCloud is here to support you. With mobile apps for Android and iOS, you can access and manage your files from anywhere.
11. **Extensible and customizable:** If you're a do-it-yourselfer, the open source nature of ownCloud is your playground. You can customize and extend its functionality to meet your unique needs.

Therefore, in a world where data control and collaboration is essential, ownCloud emerges as your faithful companion: a user-friendly, secure and adaptable platform with your ever-changing digital needs. It's like having a swiss army knife for your data, ready to take on any task. 🌐🔒📂

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
