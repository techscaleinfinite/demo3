---
cover: ../../.gitbook/assets/USA-Dedicated-Server-12.jpg
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

# Linux VPS deployment

### <mark style="color:blue;">What's Linux VPS?</mark>

The Linux Virtual Private Server (VPS) is your personal virtual environment that you can set up in mere seconds, connect to, and utilize. Similar to your personal computer, it offers a controlled space for your projects, experiments, and applications.

**Key Points:**

1. **Virtual Private Server:** A virtual instance on a physical server, providing a dedicated environment for your activities.
2. **Swift Setup:** Within seconds, you can launch your Linux VPS, skipping the traditional hardware and OS setup.
3. **Connect & Use:** Access your VPS remotely, just like using your computer, through a terminal or SSH connection.
4. **Controlled Environment:** Customize your VPS with the software, configurations, and tools you need.
5. **Isolation:** Your VPS is isolated from other users' activities, ensuring privacy and security.

### <mark style="color:blue;">**Working in Brief:**</mark>

1. **Server Virtualization:** The physical server is divided into multiple virtual compartments, each functioning independently.
2. **VPS Creation:** You select your preferred Linux distribution and configuration, and the VPS is created swiftly.
3. **Remote Access:** Via SSH or a terminal, you access your VPS from anywhere.
4. **Customization:** Install software, deploy applications, and tailor the environment to your liking.
5. **Utilization:** Run websites, applications, experiments, and more within your controlled VPS space.

With Linux VPS, you gain a versatile, isolated environment that's ready to adapt to your needs – all without the hassle of hardware setup.

### &#x20;<mark style="color:blue;">Steps And Procedure</mark>

* &#x20;**Docker image of this application consists of following layers**&#x20;

```
'FROM ubuntu:20.04' Taking ubuntu:20.04 as the base image.

And updating and installing all the required packages like 'supervisor' a system that allows users to monitor and control a number of processes 'nginx' 'xz-utils' 'dbus-x11' 'dbus-x11' and important tools like 'net-tools'  for controlling the network subsystem of the Linux kernel.

Then installed the 'vim-tiny' 'firefox' 'lxde' and 'vnc' virtual network computing software is very important for this application.

And 'copying' all the required files to the image.

Exposing the port '80' to access the vps.

```

#### Deploy LinuxVPS on Scaleinfinite

* &#x20;Go to create apps page and Search <mark style="color:orange;">scaleinfinite/linuxvps</mark> on the search bar.
* Click on install button.
* &#x20;Fill all the required fields.
* &#x20;click on Advanced.
* Click on the Install button.
* You will be redirected to My Apps page, Here you can find all the applications you deployed.
* Copy the Linuxvps application Hostname without NodePort and search the Url.
* &#x20;Now you can see a similar window like this.
* &#x20;From pressing the LADE symbol button you can access to terminal and file-system etc..,

### &#x20;<mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------ |
| [`Linux VPS`](https://hub.docker.com/r/scaleinfinite/linuxvps)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                              |
| ----------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: Linux(you can put any name)</mark> |

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

<mark style="color:purple;">**Step-by-Step Guide to Linux Vps Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`linux vps`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `linux`
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

By following these steps, you can effortlessly deploy an Linux Vps instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 151320.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 151425.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.

{% embed url="https://youtu.be/34WoUxoQvzY" %}



### <mark style="color:blue;">FAQ</mark>

**About Linux VPS image we used.**

This image is maintained by the scale infinite.

**Do the image secure to use?**

The image is created and verified by the scale infinite. it is a 100% secure image.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
