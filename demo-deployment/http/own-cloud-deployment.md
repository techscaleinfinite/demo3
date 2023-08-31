---
cover: ../../.gitbook/assets/ownCloud-Trademark.png
coverY: 0
---

# Own Cloud Deployment

### <mark style="color:blue;">What's  OWNCLOUD?</mark>

<mark style="color:orange;">"OwnCloud" is an open-source software platform that provides file synchronization and sharing services</mark>. It allows individuals and organizations to set up their own cloud storage solution on their servers, giving them control over their data and enabling secure file access and sharing

### <mark style="color:blue;">**How It Work:**</mark>

**1. **<mark style="color:orange;">**File Synchronization and Sharing**</mark>**:** ownCloud enables users to synchronize files and folders across multiple devices, such as computers, smartphones, and tablets. It allows seamless access to files from anywhere, promoting collaboration and productivity.

**2. Self-Hosted Solution:** Unlike using third-party cloud storage providers, ownCloud allows users to host their cloud storage platform on their own servers or infrastructure. This gives users control over their data, privacy, and security.

<mark style="color:orange;">**3. User-Friendly Web Interface:**</mark> ownCloud provides a user-friendly web interface where users can upload, organize, and manage their files. The interface resembles traditional file managers, making it intuitive for users to navigate and interact with their files.

**4. Access Control and Sharing:** Users can easily share files and folders with others, setting specific permissions for access and editing. This makes it suitable for collaborative work environments or sharing content with clients, partners, or friends.

<mark style="color:orange;">**5. Security and Encryption:**</mark> ownCloud prioritizes data security. It offers encryption for data at rest and in transit, ensuring that files are protected from unauthorized access. Additionally, users can manage encryption keys themselves for added security.

**6. Integration with External Storage:** ownCloud can be configured to connect to external storage sources such as FTP, Amazon S3, Google Drive, and more. This allows users to centralize their data from various sources within their ownCloud instance.

**7. App Ecosystem:** ownCloud provides an ecosystem of apps and plugins that extend its functionality. Users can enhance their cloud storage experience with features like calendars, contacts, document editing, and more.

**8. Collaborative Editing:** ownCloud supports collaborative editing of documents, allowing multiple users to work on the same document simultaneously. Changes are synchronized in real-time, fostering collaboration and reducing the need for email attachments.

**9. File Versioning:** Users can keep track of file versions and revert to previous versions if needed. This feature is particularly useful for maintaining document history and tracking changes.

**10. Mobile Apps:** ownCloud offers mobile apps for Android and iOS, enabling users to access and manage their files on the go.

**11. Extensible and Customizable:** ownCloud's open-source nature allows developers to customize and extend its functionality to meet specific requirements.

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
