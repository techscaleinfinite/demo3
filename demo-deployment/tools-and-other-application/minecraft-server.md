---
cover: ../../.gitbook/assets/500399.webp
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

# Minecraft Server

### <mark style="color:blue;">Whats Minecraft Server?</mark>

ScaleInfinite offers a personalized Minecraft server, exclusively for you and your friends, ensuring an uninterrupted and immersive gaming experience.

**Key Points:**

1. <mark style="color:orange;">**Dedicated Gaming Space**</mark>**:** Enjoy a dedicated server environment exclusively for Minecraft.
2. **Friends Inclusion:** Invite friends to join and play together on your private server.
3. <mark style="color:orange;">**24/7 Availability**</mark>**:** The server is accessible anytime, allowing gaming day and night.
4. **Custom Rules:** Set your own rules, mods, and gameplay options for a unique experience.
5. <mark style="color:orange;">**Data Security**</mark>**:** Your gaming progress and interactions remain secure within your private server.

### <mark style="color:blue;">**Working in Brief:**</mark>

1. <mark style="color:orange;">**Deployment:**</mark> Deploy your personalized Minecraft server on ScaleInfinite.
2. **Access Control:** Invite friends by sharing server IP and port information.
3. <mark style="color:orange;">**Gameplay**</mark>**:** Players connect to the server using the provided details.
4. **Shared Adventure:** Collaborate with friends, explore, build, and engage in Minecraft activities.
5. <mark style="color:orange;">**Admin Control**</mark>**:** As the server owner, you manage settings, mods, and player access.

ScaleInfinite's personal Minecraft server provides an ideal platform for seamless and exclusive gaming sessions with friends. It fosters creativity, collaboration, and hours of enjoyment in a safe and controlled environment.

### &#x20;<mark style="color:blue;">Steps And Procedure</mark>&#x20;

* &#x20;**This deployment uses the official Minecraft Docker image.**
* &#x20;Go to create apps page and Search on the search bar.
* &#x20;Click on install button.
* &#x20;Fill all the reqired fields.
* click on Advanced.
* &#x20;Click on the Install button.
* &#x20;You will be redirected to My Apps page, Here you can find all the applications you deployed.
* &#x20;Copy the minecraft application Hostname without NodePort and search the Url.

### <mark style="color:blue;">Installation</mark>

| PRODUCT NAME                                                                                                            |
| ----------------------------------------------------------------------------------------------------------------------- |
| [`minecraft`](https://hub.docker.com/r/itzg/minecraft-server)<mark style="background-color:yellow;">👈(click me)</mark> |

| Application name                                                                   |
| ---------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: micecraft1(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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

<mark style="color:purple;">**Step-by-Step Guide to Minecraft Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`minecraft`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `minecaft1`
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `TCP`
   * Port:&#x20;
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

By following these steps, you can effortlessly deploy an Minecraft instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">FAQ</mark>

**About minecraft image we used.**

This is the official minecraft image.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going! &#x20;
