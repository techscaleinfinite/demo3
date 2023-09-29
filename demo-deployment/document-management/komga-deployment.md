---
cover: ../../.gitbook/assets/637a3fb4f1196.png
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

# 📙 Komga Deployment

### <mark style="color:blue;">What's komga?</mark>

<mark style="color:orange;">**Komga: Your Gateway to the World of Comics and Mangas**</mark>

<mark style="color:orange;">Are you an avid comics or mangas enthusiast? Look no further than</mark> <mark style="color:orange;"></mark>_<mark style="color:orange;">Komga</mark>_<mark style="color:orange;">, your free and open-source comics/mangas server. Here's what sets it apart:</mark>

📚 **Easy Browsing, Anywhere:**

* Access your libraries, series, and books effortlessly through a responsive web UI. Whether you're on a desktop, tablet, or phone, Komga adapts to your needs.

📖 **Organize with Finesse:**

* Tired of clutter? Komga lets you create collections and read lists to keep your library in pristine order. Say goodbye to the chaos.

📋 **Metadata Mastery:**

* Take control by editing metadata for your series and books. Komga even automatically imports embedded metadata, saving you time and effort.

🔖 **Immersive Reading:**

* Dive into the world of comics with Komga's web reader, offering multiple reading modes to suit your preferences.

👤 **Multi-User Management:**

* Share the love for comics with friends and family. Komga allows you to manage multiple users, control access per library, set age restrictions, and apply label restrictions.

📡 **The Power of REST:**

* Komga offers a REST API, opening doors to numerous community tools and scripts that can enhance your comics/mangas experience.

📥 **Effortless Downloads:**

* Want to enjoy your favorite comics offline? Komga lets you download book files, entire series, or read lists with ease.

🔍 **No More Duplicates:**

* Say farewell to duplicates! Komga detects duplicate files and even goes the extra mile by identifying duplicate pages, ensuring your collection stays tidy.

📥 **Seamless Imports:**

* Adding new content is a breeze with Komga. Import books from outside your libraries directly into your series folder without a hitch.

🚀 **ComicRack Compatibility:**

* For ComicRack users, Komga seamlessly imports cbl read lists, making your transition smooth and painless.

Join the Komga community today and embark on an adventure through the captivating world of comics and mangas. Your next favorite read awaits!

### <mark style="color:blue;">**How It Works**</mark>

&#x20;<mark style="color:orange;">**How Komga Works: Unveiling the Magic Behind Your Comics and Mangas Server**</mark>

<mark style="color:orange;">Ever wondered how Komga, your comics and mangas server, conjures up a seamless reading experience? Let's peel back the curtain and discover the inner workings:</mark>

1. **Library Creation:** Your journey begins with library creation. You organize your comics and mangas by creating libraries. Each library acts as a container for your beloved series and books.
2. **Series and Books:** Within each library, you categorize your comics into series and individual books. This hierarchy keeps your collection structured and easy to navigate.
3. **Metadata Management:** Komga allows you to edit metadata for your series and books. You can add details like titles, authors, covers, and more. Don't worry about manual input; Komga can automatically import embedded metadata to save you time.
4. **Collections and Read Lists:** Create collections and read lists to further organize your comics. Collections group series by genre, theme, or any category you desire. Read lists let you curate a sequence of comics for binge-reading.
5. **Responsive Web UI:** Access your library through a responsive web UI. It adapts to your device, whether you're using a desktop computer, tablet, or smartphone. No matter where you are, your comics are at your fingertips.
6. **Web Reader:** Komga's web reader offers an immersive reading experience. You can choose from various reading modes that suit your preferences, ensuring your comics look just the way you like them.
7. **User Management:** Share the joy of comics with friends and family. Komga supports multiple users, each with their access control. You can set age restrictions and apply label restrictions to curate the content available to different users.
8. **REST API:** For the tech-savvy, Komga boasts a REST API that opens up a world of possibilities. Various community tools and scripts can interact with Komga, enhancing your comics/mangas adventure.
9. **Downloads and Imports:** Komga makes it easy to download comics for offline enjoyment. You can download individual book files, entire series, or read lists. Plus, if you have content outside your libraries, you can import it directly into your series folder.
10. **Duplicate Detection:** Komga keeps your library clutter-free by detecting duplicate files and pages. Say goodbye to redundancy.
11. **ComicRack Compatibility:** If you're transitioning from ComicRack, Komga seamlessly imports cbl read lists, ensuring a smooth shift to your new comics haven.

With these enchanting mechanisms, Komga transforms your comics and mangas into an organized, accessible, and delightful collection. Dive into the world of comics with Komga and relish the magic of an impeccable reading experience!

### <mark style="color:blue;">Steps And Procedure</mark>

<mark style="background-color:green;">**This deployment utilizes the official komgaDocker image. Here's a step-by-step guide to get you started:**</mark>

1. Begin by navigating to the "Create Apps" page and use the search bar to find the [l](https://hub.docker.com/r/linuxserver/your\_spotify)[gotson/komga](https://github.com/gotson/komga)   application.
2. Click on the "Install" button to initiate the installation process.
3. Fill in all the required fields with the necessary information.
4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
5. After making your selections, press the "Install" button to proceed.
6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
7. Copy the Hostname of the  Komga application without the NodePort and paste it into your preferred browser's address bar.
8. Voilà! You're now able to access the  Komga webpage and explore its content.

By following these straightforward steps, you'll have successfully deployed the  Komga application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                        |
| ----------------------------------------------------------------------------------------------------------------------------------- |
| [komga ](https://hub.docker.com/r/gotson/komga)  <mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                              |
| ----------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: komga(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td>25600</td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

| Install with Default                                                                                                                                        | Advanced                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">(select this if you want install with default settings if don't have environment value and working directory)</mark> | <mark style="background-color:yellow;">(select this if you want to go with advanced settings, where you select you own environment value and working directory)</mark> |

If you choose Advanced option:

| ENV VARIABLE                                                            |
| ----------------------------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> |

| WORKING DIR                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------ |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p>                                  |
| <mark style="color:red;">Here use ( use the path after   " :"   or the right side after "=")</mark>                      |
| <p>--mount type=bind,source=/path/to/config, target=/config<br>--mount type=bind,source=/path/to/data,target=/data \</p> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to komga Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`komga`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `komga`
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: 25600
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
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an  Komga instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-12 115536.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-12 115514.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-12 121041.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-12 121248.png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About** Komga **image we used.**

This is the officia Komga image.

**Can I deploy my own** Komga **image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going
