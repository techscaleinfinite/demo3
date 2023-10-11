---
description: >-
  The powerhouse behind Wikipedia and countless collaborative sites. Empower
  users to collectively create and manage content with version history for
  seamless edits.
cover: ../../.gitbook/assets/MediaWiki-2020-logo-horizontal.svg.png
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

<mark style="color:orange;">MediaWiki is a versatile and open-source wiki software application developed by the Wikimedia Foundation, the same organization behind Wikipedia. It's renowned for powering Wikipedia and numerous other collaborative websites across the internet. MediaWiki is engineered to facilitate the creation and management of wikis, which are platforms where users collectively contribute and edit content. Here's a deeper look at some key features and facets of MediaWiki:</mark>

**Collaborative Editing**: At the core of MediaWiki is its ability to foster collaboration. Multiple users can seamlessly work together on content creation and editing. They have the freedom to make modifications to existing articles, introduce fresh content, and engage in discussions regarding these alterations on article talk pages.

**Version History**: Every alteration made to a page within MediaWiki is meticulously tracked and stored in a comprehensive version history. This version history is an invaluable resource that permits users to peruse previous iterations of a page, compare changes between versions, and even revert back to prior renditions when deemed necessary.

**Content Structuring**: MediaWiki excels at structuring content. Information is neatly organized into articles, which can then be effectively grouped into categories. Users are empowered to not only craft and refine articles but also to categorize them, forging a structured hierarchy through links and templates.

**User Accounts**: MediaWiki introduces user accounts, which grant users additional privileges in the editing and administrative realms. Registered users benefit from features like personal user pages, watchlists to monitor page modifications, and user talk pages that facilitate communication within the community.

**Markup Language**: MediaWiki employs a user-friendly markup language. It is designed to be intuitive and accessible, featuring straightforward syntax for text formatting, hyperlink creation, image embedding, and other formatting elements.

**Media Integration**: MediaWiki seamlessly incorporates various media types, encompassing images, audio files, and videos. Users can effortlessly upload these multimedia elements to enrich the content of articles, enhancing both visual appeal and informational depth.

MediaWiki stands as a testament to collaborative knowledge creation and dissemination. Its user-friendly interface, extensive features, and adaptability make it an ideal choice for not only Wikipedia but a myriad of collaborative projects and knowledge-sharing platforms across the digital landscape

### <mark style="color:blue;">**How It Works**</mark>

<mark style="color:orange;">**Content Creation and Editing**</mark><mark style="color:orange;">: One of the fundamental features of MediaWiki is its robust content creation and editing capabilities. Users, provided they have the appropriate permissions, can author new articles or modify existing ones. Articles are typically composed using a markup language, which simplifies tasks like text formatting, hyperlink creation, and media inclusion.</mark>

**Version Control:** In the realm of version control, MediaWiki excels. It meticulously records and archives every alteration made to an article, establishing a comprehensive version history. This historical record encompasses details such as the identity of the editor, the nature of the changes, and the timestamps of modifications. This version history serves as a valuable resource, allowing users to revisit and even revert to prior iterations when necessary.

**User Contributions:** MediaWiki fosters a sense of community by offering registered users the opportunity to create personalized user pages. These pages serve as spaces where users can introduce themselves to the community and showcase their contributions to the wiki. Additionally, user talk pages provide a means of communication between users, facilitating discussions and collaborations.

**Categories and Links**: To enhance the organization of content, MediaWiki allows articles to be systematically categorized. Moreover, articles can be interlinked, creating a web of interconnected knowledge within the wiki. This interlinking simplifies navigation and promotes the discoverability of related information.

**Templates:** Templates are a powerful tool in the MediaWiki arsenal. They are reusable content blocks that can be seamlessly integrated into articles. Templates find application in a variety of contexts, including the creation of infoboxes, citation formats, and other standardized content elements.

**Searching**: The built-in search engine equips users with a powerful tool for locating articles. By inputting keywords, users can swiftly retrieve a list of pertinent articles, streamlining the process of finding relevant information.

**Media Integration:** MediaWiki facilitates the integration of multimedia elements, encompassing images, audio clips, and video files. Users can effortlessly upload and embed these media components within articles, enriching the content and making it more engaging.

**Recent Changes:** The "Recent Changes" page is an indispensable feature that offers a real-time glimpse into the wiki's activity. It presents a chronological list of the most recent edits made across the entire wiki, providing users with an efficient means of monitoring changes and staying abreast of developments.

MediaWiki stands as a testament to the collaborative spirit of online knowledge sharing. With its user-friendly interface and versatile feature set, it empowers communities to create, curate, and disseminate knowledge effectively.

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

    By following these straightforward steps, you'll have successfully deployed the  media wiki application and gained access to its features through a seamless and user-friendly process.

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

| WORKING DIR                                                                                       |
| ------------------------------------------------------------------------------------------------- |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p>           |
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                           |
| <p></p><pre class="language-console"><code class="lang-console">/var/www/html/sites
</code></pre> |

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
       * <mark style="color:red;">Here use ( use the path after   " :"  )</mark>
       *

           ```console
           /var/www/html/sites
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an media wiki instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-01 152224.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-01 152718.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-01 152346.png" alt=""><figcaption></figcaption></figure>

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

<details>

<summary>Category</summary>

Kubernetes, cloud computing, DevOps, cloud services, hosting platform, container orchestration, cloud infrastructure, cloud deployment, cloud management, cloud technology, cloud solutions&#x20;

</details>
