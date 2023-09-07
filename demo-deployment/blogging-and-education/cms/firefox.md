---
cover: ../../../.gitbook/assets/208-2080292_firefox-logo.png
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

# 🦊 Firefox

### <mark style="color:blue;">What's firefox?</mark>

Firefox is a popular, open-source web browser developed by Mozilla. It provides users with a versatile and secure online browsing experience. Here's an overview of what Firefox is all about:

**1. Browsing the Web:**

* Firefox serves as a web browser, allowing users to access and view websites on the internet. Users can navigate to their favorite sites by typing URLs or using search engines.

**2. Open Source:**

* Firefox is an open-source software, meaning its source code is freely available to the public. This fosters transparency, community contributions, and innovation in browser development.

**3. User-Friendly Interface:**

* Firefox features a user-friendly and customizable interface. Users can personalize their browser's appearance by changing themes and adding extensions.

**4. Cross-Platform Compatibility:**

* Firefox is available on multiple platforms, including Windows, macOS, Linux, iOS, and Android. Users can access their bookmarks, history, and settings across devices.

**5. Security and Privacy:**

* Mozilla places a strong emphasis on user security and privacy. Firefox includes features like Enhanced Tracking Protection, which blocks third-party trackers, and strict sandboxing for added security.
* The browser also offers Private Browsing mode, which prevents the storage of browsing history, cookies, and site data.

**6. Extensibility:**

* Firefox supports a wide range of add-ons and extensions that enhance its functionality. Users can install extensions for ad-blocking, password management, and more.

**7. Tab Management:**

* Firefox provides robust tab management features, including the ability to pin tabs, group tabs into tab containers, and restore previous sessions.

**8. Performance:**

* Mozilla continually optimizes Firefox for faster page loading and smoother performance. It also supports cutting-edge web technologies for a seamless browsing experience.

**9. Developer Tools:**

* Firefox offers a comprehensive set of developer tools, making it a favorite among web developers for debugging and inspecting web pages.

**10. Accessibility:** - Firefox is committed to accessibility, ensuring that individuals with disabilities can use the browser effectively. It includes features like screen reader support and keyboard navigation.

**11. Updates and Community:** - Firefox receives regular updates to address security vulnerabilities, improve performance, and introduce new features. Mozilla engages with a global community of users and developers to gather feedback and drive browser development.

**12. Privacy Features:** - Firefox includes features like Firefox Monitor, which alerts users if their email addresses are part of a data breach, and Facebook Container, which isolates Facebook activity to protect user privacy.

In summary, Firefox is a user-centric, open-source web browser that prioritizes user security, privacy, and customization. It offers a seamless web browsing experience while allowing users to tailor their browser to their specific needs through extensions and themes. Firefox's commitment to transparency and user-centric design makes it a popular choice among internet users worldwide.



### <mark style="color:blue;">**How It Works:**</mark>

Firefox is a web browser, kind of like a pair of magic glasses that lets you see the internet. It's made by a group called Mozilla, and they're all about making sure the internet is a safe and friendly place for everyone.

When you open Firefox, it's like opening a door to the internet world. You can type in web addresses, and Firefox will take you to those websites. You can also use it to search for things on the internet.

One cool thing about Firefox is that it's open source, which means it's built by a big community of people who share their ideas and make it better all the time. It's like a big group project to create the best web browser.

Firefox also cares a lot about your privacy and security. It has tools that stop sneaky trackers from following you around the internet and collecting your data. There's even a special mode called Private Browsing that makes sure nothing you do online is stored on your computer.

You can make Firefox look and work the way you want by adding themes and extensions. It's like decorating your magic glasses or adding superpowers to them. Some extensions can block ads, save your passwords, or do other helpful things.

Tabs in Firefox are like having multiple windows open at once. You can have lots of websites open in different tabs, and you can even organize them into groups.

Whenever you visit a website, Firefox is working behind the scenes to load all the pictures, text, and videos. It's like a super-fast delivery service for web content.

If you're a developer, Firefox has tools to help you build and test websites. It's like having a toolbox for creating cool stuff on the internet.

And just like your phone, you can use Firefox on different devices like your computer, tablet, or phone. It even syncs your bookmarks and history so you can pick up where you left off, no matter which device you're using.

In a nutshell, Firefox is like your trusty sidekick for exploring the internet. It's designed to keep you safe, give you control, and make your online adventures as enjoyable as possible.

### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official firefox Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the linuxserver/firefox application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the firefox application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the  firefox webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed the firefox application and gained access to its features through a seamless and user-friendly process.



### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                                                              |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [`firefox`<mark style="background-color:yellow;">👈(</mark>](https://hub.docker.com/r/linuxserver/firefox)<mark style="background-color:yellow;">click me,for the dockerhub image)</mark> |

| Application name                                                                  |
| --------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: jfirefox1(you can put any name)</mark> |

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

<mark style="color:purple;">**Step-by-Step Guide to joomla Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`joomla`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `joomla`
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

By following these steps, you can effortlessly deploy an  firefox instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-04 163913.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-04 164012.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-04 164043.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.

### <mark style="color:blue;">FAQ</mark>

**About joomla image we used.**

This is the official joomla image.

**Can I deploy my own media joomla with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
