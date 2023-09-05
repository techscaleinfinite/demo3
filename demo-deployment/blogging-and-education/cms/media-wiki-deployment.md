---
cover: ../../../.gitbook/assets/MediaWiki-2020-logo-horizontal.svg.png
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

# 🖥 Media Wiki Deployment

### <mark style="color:blue;">What's media wiki?</mark>

**MediaWiki** is a free and open-source wiki software application developed by the Wikimedia Foundation. It's the same software that powers Wikipedia, one of the most popular and widely used wikis on the internet. MediaWiki is designed to create and manage wikis, which are collaborative websites where users can contribute and edit content collectively. Here are some key features and aspects of MediaWiki:

1. **Collaborative Editing**: MediaWiki allows multiple users to collaborate on creating and editing content. Users can make edits to articles, add new content, and discuss changes on article talk pages.
2. **Version History**: Every change made to a page is tracked in a version history. Users can view previous versions, compare changes, and revert to older versions if necessary.
3. **Content Structuring**: Content in MediaWiki is organized into articles, which are grouped into categories. Users can create and edit articles, categorize them, and create a hierarchical structure using links and templates.
4. **User Accounts**: Users can create accounts to gain additional editing and administrative privileges. Registered users can have user pages, watchlists to track changes, and user talk pages for communication.
5. **Markup Language**: MediaWiki uses a markup language that's easy to learn and use. It includes simple syntax for formatting text, creating links, adding images, and more.
6. **Media Integration**: MediaWiki supports the integration of various media types, including images, audio, and video. Users can upload files to articles, enhancing the content.

### <mark style="color:blue;">**How It Works:**</mark>

1. **Content Creation and Editing**: Users with appropriate permissions can create new articles or edit existing ones. Articles are typically written using a markup language, which allows for easy text formatting, linking, and the inclusion of media.
2. **Version Control**: Every change made to an article is tracked and saved in a version history. This means that each article has a record of all edits, who made them, and when they were made. This version history allows users to revert to previous versions if needed.
3. **User Contributions**: Registered users often have a user page where they can introduce themselves and list their contributions. There are also user talk pages for communication between users.
4. **Categories and Links**: Articles can be organized into categories, and they can link to other articles within the wiki. This creates a web of interconnected knowledge.
5. **Templates**: Templates are reusable blocks of content that can be included in articles. They are often used for infoboxes, citations, and other standardized content.
6. **Searching**: Users can search for articles using the built-in search engine, which provides a list of relevant articles based on keywords.
7. **Media Integration**: MediaWiki supports the uploading and embedding of images, audio, and video files. This enhances the content of articles.
8. **Recent Changes**: There's a "Recent Changes" page that shows a list of the most recent edits across the entire wiki. This is a useful tool for monitoring changes and staying updated.

### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official mediawiki Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the <mark style="color:orange;">mediawiki</mark> application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the mediawiki application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the mediawiki webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed the Nginx application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------------------ |
| [`mediawiki`](https://hub.docker.com/\_/mediawiki)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                                   |
| ---------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: mediawiki1(you can put any name)</mark> |

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

<mark style="color:purple;">**Step-by-Step Guide to MEDIAWIKI Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`mediawiki`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `mediawiki`
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

By following these steps, you can effortlessly deploy an NGINX instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-01 152224.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-01 152718.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-01 152346.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About media wiki image we used.**

This is the official medi wiki image.

**Can I deploy my own media wiki image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
