---
cover: ../../../.gitbook/assets/effef.png
coverY: -71
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

# 📓 mininote deployment

### <mark style="color:blue;">What's mininote?</mark>

<mark style="color:orange;">**MiniNote: Your Secret Sanctuary for Markdown Memoirs**</mark>

Introducing _MiniNote_, the unassuming yet brilliant self-hosted gem designed for your confidential Markdown note-taking needs. Here's a sneak peek into the world of MiniNote, where simplicity meets security:

📝 **Simplicity in Complexity:**

* MiniNote is a testament to the beauty of simplicity. Behind its uncluttered interface lies a robust tool for crafting and storing Markdown-based notes.

🔒 **Fortress of Encryption:**

* Your thoughts deserve the utmost security. MiniNote takes your privacy seriously by encrypting your notes, ensuring they remain exclusively yours.

📚 **Markdown Magic:**

* Markdown aficionados rejoice! MiniNote understands your language. Craft beautifully formatted notes with ease, harnessing the power of Markdown syntax.

🏡 **Self-Hosted Sanctuary:**

* MiniNote doesn't believe in third-party custody. It's your data, and you control it. Hosting it yourself adds an extra layer of ownership and security.

🌟 **No-Frills, All Thrills:**

* MiniNote isn't about flashy features. It's about getting down to business—taking notes with minimal distractions and maximal productivity.

🔐 **Data's Best Friend:**

* Your data is precious, and MiniNote treats it as such. With encryption and self-hosting, your notes are in the safest of hands—yours.

🌐 **Web-Based Wonder:**

* Access MiniNote from anywhere, anytime. Its web-based nature ensures you're never far from your thoughts.

🚀 **Effortless Efficiency:**

* MiniNote streamlines your note-taking process. Write, edit, and access your notes seamlessly, without the fuss.

In a world filled with overcomplicated note-taking apps, MiniNote stands as a beacon of simplicity and security. It's where your thoughts become encrypted masterpieces, where Markdown's elegance shines, and where you're always in control. Say hello to MiniNote, your digital sanctuary for Markdown memoirs



### <mark style="color:blue;">**How It Works:**</mark>

<mark style="color:orange;">**MiniNote: Where Security Meets Simplicity**</mark>

In the realm of digital sanctuaries, _MiniNote_ stands as a fortress of security with a dash of simplicity. Here's the lowdown on MiniNote's security features:

🔒 **Bulletproof Encryption:**

* MiniNote wraps your notes in a cloak of encryption, ensuring that both titles and content remain as secret as the recipe for grandma's cookies. It uses AES-GCM, a formidable encryption method, courtesy of the Web Crypto API.

🔐 **Password Power:**

* Remember, encryption is only as strong as your password. MiniNote lets you wield this power by using your notebook's password to derive the encryption key. Choose wisely, and your notes will be as secure as Fort Knox.

🌐 **End-to-End-ish:**

* While MiniNote takes encryption seriously, it's honest about its limitations. It encrypts your notes before they travel to the server, but it's not quite "NSA-proof." The server might catch a glimpse of your password when creating a new notebook. Think of it as locking your diary with a sturdy padlock, but the locksmith knows the design.

⚔️ **Decent Security:**

* MiniNote doesn't make grandiose claims, but it does aim for a decent level of security. It's your digital safe haven, not a spy movie prop.

In the world of note-taking apps, MiniNote strikes a balance between robust security and user-friendly simplicity. Your notes are encrypted, your thoughts are guarded, and your Markdown memoirs are in safe hands. Welcome to MiniNote, where security meets simplicity with a touch of wit.

### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official mininote Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the [n1try/mininote](https://hub.docker.com/r/n1try/mininote) application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the  MiniNote  application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the   MiniNote webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed the  MiniNote application and gained access to its features through a seamless and user-friendly process.



### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                                                                                                           |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [mini n](https://hub.docker.com/r/n1try/mininote)ote  [<mark style="background-color:yellow;">👈(</mark>](https://hub.docker.com/r/linuxserver/firefox)<mark style="background-color:yellow;">click me,for the dockerhub image)</mark> |

| Application name                                                                  |
| --------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: mini note(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">3000</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

| Install with Default                                                                                                                                        | Advanced                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">(select this if you want install with default settings if don't have environment value and working directory)</mark> | <mark style="background-color:yellow;">(select this if you want to go with advanced settings, where you select you own environment value and working directory)</mark> |

If you choose Advanced option:

| ENV VARIABLE                                                            |
| ----------------------------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> |

| WORKING DIR                                                                                        |
| -------------------------------------------------------------------------------------------------- |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p>            |
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                            |
| <p></p><pre class="language-bash"><code class="lang-bash">-v mininote-data:/app/data
</code></pre> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to mininote Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`mininote`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `mininote`
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `3000`
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
           -v mininote-data:/app/data
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an  MiniNote instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-11 173542.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-11 173606.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-11 173715.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.

### <mark style="color:blue;">FAQ</mark>

**About** MiniNote **image we used.**

This is the official  MiniNote mage.

**Can I deploy my own media** MiniNote **with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions, notes

</details>
