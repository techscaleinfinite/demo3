---
cover: ../../.gitbook/assets/drupal-vector-logo-2022.png
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

# Drupal deployment

### <mark style="color:blue;">What's Drupal?</mark>

Drupal is a powerful, open-source web content management system (CMS) built using the PHP scripting language. It offers a versatile platform for creating, managing, and customizing websites to meet your specific needs.

**Key Points:**

1. **Open-Source CMS:** Drupal is freely accessible, providing a foundation for website development and management.
2. <mark style="color:orange;">**PHP-Powered**</mark>**:** The core of Drupal is written in PHP, a versatile scripting language.
3. **Modularity:** Drupal's modular architecture allows you to add and customize features using modules.
4. <mark style="color:orange;">**Customization**</mark>**:** Tailor your site's appearance and functionality with themes and modules.
5. **Community-Driven:** A thriving community contributes to Drupal's development, providing updates, support, and resources.

### <mark style="color:blue;">**Working in Brief**</mark>

1. <mark style="color:orange;">**Content Creation**</mark>**:** Easily create and organize content using Drupal's user-friendly interface.
2. **Modular Architecture:** Add functionalities with modules that offer specific features or integrations.
3. <mark style="color:orange;">**Themes & Appearance**</mark>**:** Customize your site's look and feel with themes, ensuring a unique design.
4. **PHP Processing:** PHP processes user requests, dynamically generating web pages and content.
5. <mark style="color:orange;">**Community Support**</mark>**:** Benefit from a community of developers and users providing updates, solutions, and enhancements.

Drupal empowers website management by providing flexibility, scalability, and a robust ecosystem of modules and themes. Its open-source nature and dedicated community make it a versatile choice for various web projects.

### &#x20;<mark style="color:blue;">Steps And Procedure</mark>

* &#x20;<mark style="background-color:orange;">**This deployment uses the official Drupal Docker image.**</mark>
* &#x20;Go to create apps page and Search <mark style="background-color:orange;">Drupal</mark> on the search bar.
* Click on install button.
* &#x20;Fill all the required fields.
* &#x20;click on Advanced.
* &#x20;Click on the Install button.
* &#x20;You will be redirected to My Apps page, Here you can find all the applications you deployed.
* &#x20;Copy the Drupal application Hostname without NodePort and search the Url.
* &#x20;Now you can access the Drupal login page.
* &#x20;Then you will be redirected to the Drupal dashboard page.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------ |
| [`drupal`](https://hub.docker.com/\_/drupal)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

| Application name                                                               |
| ------------------------------------------------------------------------------ |
| <mark style="background-color:yellow;">Eg: drupal(you can put any name)</mark> |

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

<mark style="color:purple;">**Step-by-Step Guide to Drupal Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`drupal`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `drupal`
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

By following these steps, you can effortlessly deploy an drupal instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 155639 (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 155724 (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 160110 (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 160414 (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/spaces_tKO1h8ymGqNtYiKTJ8WZ_uploads_kuTabiFuRQL5mCpFhJ1f_Screenshot 2023-08-12 154105 (1).webp" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:blue;">FAQ</mark>

**About Drupal image we used.**

This is the official Drupal image.

**Is the Database inbuilted in the same image ?**

No, you need to add your database while you are login and setting your website.

**Can i deploy older version of drupal or my own modified drupal image ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
