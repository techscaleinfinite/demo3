# Book Stack

### <mark style="color:blue;">What's is book stack?</mark>

BookStack" is an open-source platform for creating and managing documentation, wikis, and knowledge bases. It provides a user-friendly interface for organizing and sharing information within an organization, team, or community. Here's a brief overview of what BookStack is and how it works:

1. **Documentation Platform**: BookStack is designed to help users create and maintain structured documentation and knowledge bases. It's often used for creating internal wikis, project documentation, user manuals, and more.
2. **Hierarchical Structure**: BookStack uses a hierarchical structure of "Books," "Chapters," and "Pages" to organize content. "Books" can contain multiple "Chapters," and each "Chapter" can contain multiple "Pages." This structure makes it easy to categorize and manage content.
3. **Rich Editing Tools**: BookStack provides a WYSIWYG (What You See Is What You Get) editor that allows users to format text, insert images, create links, embed media, and more. This makes it simple to create visually appealing and informative conten

### <mark style="color:blue;">**How It Works:**</mark>

1. **Configuration**: You define the services you want to include in your Homer dashboard using a YAML configuration file. This configuration file lists the names, URLs, and icons of the services you want to access.
2. **Dashboard Interface**: Once you've set up the configuration, you can access your Homer dashboard through a web browser. The dashboard presents an organized view of your services, making it easy to find and launch them.
3. **Service Accessibility**: Each service entry on the dashboard typically includes an icon, name, and URL link. Clicking on a service's icon or name opens a new tab or window in your browser and directs you to the specified service's URL.
4. **Customization**: Homer allows you to customize the appearance of the dashboard by choosing different themes, layouts, and colors to match your preferences.
5. **Quick Access**: By using Homer, you can eliminate the need to remember individual URLs or bookmarks for various self-hosted services. Instead, you have a centralized place to access everything.

### <mark style="color:blue;">Steps And Procedure</mark>

* &#x20;<mark style="background-color:purple;">**This deployment uses the official homer bookstack image.**</mark>
* &#x20;Go to create apps page and Search  on the search bar.
* &#x20;Click on install button.
* &#x20;Fill all the required fields.
* &#x20;click on Advanced.
* Click on the Install button.
* You will be redirected to My Apps page, Here you can find all the applications you deployed.
* &#x20;Copy the nginx application Hostname without NodePort and search the Url.
* &#x20;Now you can able to access the nginx webpage.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                  |
| --------------------------------------------------------------------------------------------------------------------------------------------- |
| [bookstack](https://hub.docker.com/r/linuxserver/bookstack)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                                  |
| --------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: bookstack(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td>-</td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>3306</td></tr></tbody></table>

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

<mark style="color:purple;">**Step-by-Step Guide to bookstack Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name: bookstack</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: bookstack
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: TCP
   * Port: 3306
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

By following these steps, you can effortlessly deploy an HOMER instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About bookstack image we used.**

This is the official bookstack image.

**Can I deploy my own bookstack image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
