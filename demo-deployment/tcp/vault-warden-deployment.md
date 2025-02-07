---
description: >-
  Vaultwarden, formerly known as Bitwarden_RS, is a self-hosted password manager
  offering enhanced privacy and control. Explore this open-source project
  focused on data security.
cover: ../../.gitbook/assets/images (2).jpg
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

# 🖥 Vault Warden Deployment

### <mark style="color:blue;">What's is vault warden?</mark>

<mark style="color:orange;">Introducing Vaultwarden, the new identity of the project formerly known as "Bitwarden\_RS." Its primary mission? To provide you with an alternative to the official Bitwarden password manager, putting the power back in your hands to host and manage your password vault in a self-hosted environment.</mark> Let's dive into the core aspects of Vaultwarden:

**Self-Hosted Password Management:** Vaultwarden empowers you, whether you're an individual or part of an organization, to take control. You can establish and maintain your very own instance of a password manager, giving you the keys to your data's kingdom. It's all about managing your password vault on your terms.

<mark style="color:red;">**Open Source Awesomeness**</mark>**:** Vaultwarden wears its open-source badge with pride. What does this mean for you? It's like having a see-through vault. The source code is out there for everyone to inspect, contribute to, and make better. It's like having a community of security experts looking out for you.

<mark style="color:blue;">**Security Fortified:**</mark> Vaultwarden doesn't mess around when it comes to security. It's like having an impenetrable vault door for your digital secrets. It uses robust encryption techniques, including end-to-end encryption, which means your passwords and sensitive info are locked down and guarded like precious treasures.

<mark style="color:red;">**Access Anywhere, Anytime:**</mark> Vaultwarden is your password vault on the move. Whether you're on a laptop, a smartphone, or a tablet, it's got your back. Browser extensions, mobile apps, and desktop clients are there to ensure your passwords are accessible no matter where you are.

<mark style="color:yellow;">**Browser Bliss**</mark>**:** Vaultwarden offers nifty browser extensions. It's like having your butler fetch your passwords for you. These extensions fill in passwords automatically and let you manage your logins right from your browser. No more typing in those long and complicated passwords.

<mark style="color:yellow;">**Double Security with 2FA**</mark>**:** Vaultwarden knows two locks are better than one. That's why it supports two-factor authentication (2FA). It's like having a moat and a drawbridge around your castle. This extra layer of protection keeps the bad guys at bay.

In a nutshell, Vaultwarden is your self-hosted password guardian. It's all about open-source goodness, top-notch security, and access wherever and whenever you need it. Say goodbye to password hassles and hello to privacy and data security. It's like having your very own digital Fort Knox. Give Vaultwarden a spin and take back control of your passwords.

### <mark style="color:blue;">**How It Works**</mark>

<mark style="color:orange;">Vaultwarden, formerly known as Bitwarden\_RS, operates as a self-hosted password management solution, offering users a secure and controlled environment to manage their passwords and sensitive information. Here's a detailed breakdown of how it functions:</mark>

1. <mark style="color:green;">**Server Setup**</mark><mark style="color:green;">:</mark> To initiate your Vaultwarden journey, you must establish a server where the Vaultwarden application will reside. This server can be either your dedicated hardware or a cloud-based instance, depending on your preferences and requirements.
2. <mark style="color:yellow;">**Installation**</mark><mark style="color:yellow;">:</mark> The next step involves installing the Vaultwarden application on your chosen server. This installation process encompasses the deployment of critical software components, including the Vaultwarden server itself, a web server (commonly Nginx), and a database (typically PostgreSQL). These components work collaboratively to ensure the seamless operation of Vaultwarden.
3. <mark style="color:orange;">**Database Storage**</mark><mark style="color:orange;">:</mark> Vaultwarden relies on a database to store a multitude of crucial elements, such as user accounts, encrypted passwords, and various sensitive data. Importantly, all data is subjected to robust encryption using advanced encryption algorithms. Furthermore, the decryption key remains exclusively in the hands of the user, enhancing data security.
4. <mark style="color:purple;">**User Accounts**</mark><mark style="color:purple;">:</mark> Users commence their Vaultwarden experience by creating individual accounts on your self-hosted instance. Each user account is fortified by a master password, which only the respective user knows. This master password plays a pivotal role in deriving the encryption key responsible for both the encryption and decryption processes of the stored data.
5. <mark style="color:orange;">**End-to-End Encryption**</mark><mark style="color:orange;">:</mark> As users begin adding passwords and other essential items to their Vaultwarden accounts, the data is encrypted right at the client's end. This encryption process relies on the user's master password and the encryption key derived from it. Once encrypted, this data is securely transmitted to the Vaultwarden server.

Vaultwarden's design places a paramount emphasis on data security, privacy, and user control. By facilitating self-hosting, robust encryption practices, and client-side data protection, Vaultwarden empowers users to confidently manage their passwords and sensitive information in a secure and personalized environment.

### <mark style="color:blue;">Steps And Procedure</mark>

*   &#x20;<mark style="background-color:purple;">**This deployment utilizes the official Vault warden Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the <mark style="color:orange;">vaultwarden/server</mark> application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the vaultwarden application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the vaultwarden webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed the vaultwardem application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                  |
| --------------------------------------------------------------------------------------------------------------------------------------------- |
| [vault varden](https://hub.docker.com/r/vaultwarden/server)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                                     |
| ------------------------------------------------------------------------------------ |
| <mark style="background-color:yellow;">Eg: vault warden(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">80</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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
| <p></p><pre class="language-sh"><code class="lang-sh">-v /vw-data/:/data/
</code></pre> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to vault watden Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name: vault warden</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: vault warden 1
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
       *

           ```sh
           -v /vw-data/:/data/
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an vault warden instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 145538.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 145621.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 145750.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-31 145921.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About vault warden image we used.**

This is the official vault warden image.

**Can I deploy my own vault warden image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, vault warden

</details>
