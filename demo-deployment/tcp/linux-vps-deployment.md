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

# 🖥 Linux VPS deployment

### <mark style="color:blue;">What's Linux VPS?</mark>

A Linux Virtual Private Server (VPS) serves as your own personal virtual environment, offering a wealth of advantages for your projects and experiments. Here are some key points to keep in mind:

1. **Virtual Private Server**: A Linux VPS is essentially a virtual instance running on a physical server. It's like having your dedicated space in the digital realm, free from the limitations of shared hosting.
2. **Swift Setup**: One of the most appealing aspects of a Linux VPS is its rapid deployment. In a matter of seconds, you can launch your VPS. Gone are the days of dealing with the hardware setup or the intricacies of configuring the operating system.
3. **Connect & Use**: Just like your personal computer, you can access your Linux VPS remotely. This is typically done through a terminal or an SSH (Secure Shell) connection. It's as if you're sitting in front of your VPS, enabling you to perform tasks, manage files, and run applications seamlessly.
4. **Controlled Environment**: With a Linux VPS, you have complete control over your environment. You can customize it to your heart's content, installing the software, configuring settings, and utilizing the tools that align with your specific needs. It's your digital canvas to paint with your preferences.
5. **Isolation**: One significant advantage of a Linux VPS is the isolation it provides. Your VPS operates independently of other users' activities on the same physical server. This isolation ensures not only your privacy but also enhances security, as you don't need to worry about the actions of others impacting your work.

In summary, a Linux VPS empowers you with a virtual playground, allowing you to set up, experiment, and work on your projects with ease. Its speed of deployment, remote accessibility, customization options, and the assurance of a controlled and isolated environment make it a valuable resource for various applications. Whether you're a developer, a hobbyist, or a professional, a Linux VPS is a versatile tool in your digital arsenal.

### <mark style="color:blue;">**Working in Brief:**</mark>

Linux VPS offers a dynamic environment that empowers users with flexibility and control. Here's a breakdown of how it operates:

1. **Server Virtualization**: The physical server is essentially partitioned into distinct virtual compartments, each acting as an independent server. This virtualization technology ensures that your VPS remains isolated from others, granting you autonomy over your digital space.
2. **VPS Creation**: Getting started with a Linux VPS is a breeze. You get to choose your preferred Linux distribution and set up the configuration parameters that suit your requirements. Once configured, your VPS is swiftly created, sparing you the complexities of traditional hardware setup.
3. **Remote Access**: One of the standout features of a Linux VPS is the ability to access it remotely. Whether you're at home, in the office, or on the go, you can securely connect to your VPS using SSH (Secure Shell) or a terminal. This remote accessibility mirrors the experience of using your local machine.
4. **Customization**: Your Linux VPS is your canvas to paint with your preferences. You have the liberty to install software, deploy applications, and fine-tune the environment to match your specific needs. This level of customization ensures that your VPS becomes a tailored solution that aligns perfectly with your projects and experiments.
5. **Utilization**: The Linux VPS serves as a versatile platform where you can run websites, host applications, conduct experiments, and much more. Its controlled environment, coupled with its isolation from other users, makes it a reliable space for your digital endeavors.

In summary, a Linux VPS offers a seamless transition from physical hardware to a virtual environment, with the added benefits of rapid setup, remote accessibility, customization, and isolation. It's a valuable tool that adapts to your needs, making it a preferred choice for individuals and professionals seeking a flexible and controlled computing environment.

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

<mark style="background-color:purple;">**This deployment utilizes the official Vault warden Docker image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find the <mark style="color:orange;">scaleinfinite/linuxvps</mark> application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the <mark style="color:orange;">linuxvps</mark> application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the <mark style="color:orange;">linuxvps</mark>webpage and explore its content.

By following these straightforward steps, you'll have successfully deployed the<mark style="color:orange;">linuxvps</mark> application and gained access to its features through a seamless and user-friendly process.



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
