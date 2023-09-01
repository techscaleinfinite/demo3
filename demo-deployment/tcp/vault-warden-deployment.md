---
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

# Vault Warden Deployment

### <mark style="color:blue;">What's is vault warden?</mark>

Vaultwarden is the new name for the project that was formerly known as "Bitwarden\_RS." It aims to offer similar functionalities to the official Bitwarden password manager but allows users to host their own instance of the service for added control and privacy.

Here are the key points about Vaultwarden:

1. **Self-Hosted Password Management**: Vaultwarden allows individuals and organizations to host their own password manager instance, providing control over data storage and privacy.
2. <mark style="color:orange;">**Open Source**</mark><mark style="color:orange;">:</mark> The project is open-source, meaning that its source code is available to the public. This fosters transparency, collaboration, and security.
3. <mark style="color:orange;">**Security**</mark><mark style="color:orange;">:</mark> Vaultwarden employs strong encryption practices to secure user data. It utilizes end-to-end encryption to protect passwords and other sensitive information.
4. **Cross-Platform Support**: Vaultwarden provides browser extensions, mobile apps, and desktop clients for various operating systems, making it convenient for users to access their passwords from different devices.
5. **Browser Integration**: Browser extensions allow users to autofill passwords and manage their credentials directly from their web browsers.
6. **Two-Factor Authentication (2FA)**: Vaultwarden supports two-factor authentication, adding an extra layer of security to user accounts.

### <mark style="color:blue;">**How It Works:**</mark>

Vaultwarden (formerly Bitwarden\_RS) works as a self-hosted password management solution, allowing users to securely store, manage, and access their passwords and other sensitive information. Here's how it works:

1. **Server Setup**: To get started with Vaultwarden, you need to set up a server where the Vaultwarden application will run. This server can be your own hardware or a cloud-based instance.
2. **Installation**: You install the Vaultwarden application on the server. This involves deploying the necessary software components, which include the Vaultwarden server itself, a web server (e.g., Nginx), and a database (e.g., PostgreSQL).
3. **Database Storage**: Vaultwarden uses a database to store user accounts, encrypted passwords, and other sensitive data. The data is encrypted with strong encryption algorithms, and only the user has the decryption key.
4. **User Accounts**: Users create accounts on your self-hosted Vaultwarden instance. Each user account is protected with a master password, which is known only to the user. This master password is used to derive the encryption key used to encrypt and decrypt the stored data.
5. <mark style="color:orange;">**End-to-End Encryption**</mark><mark style="color:orange;">:</mark> When users add passwords or other items to their Vaultwarden accounts, the data is encrypted on the client side using their master password and the encryption key derived from it. This encrypted data is then sent to the Vaultwarden server.

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
