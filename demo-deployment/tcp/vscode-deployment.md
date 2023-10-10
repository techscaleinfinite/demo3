---
cover: ../../.gitbook/assets/download (6).png
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

# 💻 Vscode Deployment

### <mark style="color:blue;">What's  VsCode?</mark>

<mark style="color:orange;">Visual Studio Code, often referred to simply as VS Code, is a free and widely-used source code editor developed by Microsoft. It stands out as a versatile and feature-rich tool designed to enhance the coding experience for developers across various programming languages and platforms.</mark>

Key Features and Aspects of VS Code:

1. **Open-Source:** VS Code is an open-source software, which means its source code is freely available for developers to view, modify, and contribute to. This open nature fosters a collaborative environment and allows the community to improve and customize the editor.
2. **Cross-Platform Compatibility:** VS Code is compatible with major operating systems, including Windows, macOS, and Linux. This cross-platform support ensures that developers can use the same coding environment regardless of their OS preference.
3. **Lightweight and Fast:** Despite its extensive feature set, VS Code remains lightweight and operates with impressive speed. It's known for its quick startup time and responsiveness, making it an efficient choice for coding tasks.
4. **Rich Language Support:** VS Code provides support for an extensive range of programming languages through the use of extensions. These extensions enhance code highlighting, auto-completion, linting, and debugging capabilities tailored to specific languages.
5. **Extensions Marketplace:** VS Code boasts a vibrant extensions marketplace where users can browse and install a wide variety of extensions to customize their development environment. These extensions cover everything from additional language support to integrations with popular frameworks and tools.
6. **Integrated Development Environment (IDE) Features:** While VS Code is technically a code editor, it offers many IDE-like features through extensions. These include integrated debugging, version control (Git), terminal access, and more.
7. **Customization:** VS Code allows users to customize their editor extensively, from themes and color schemes to keybindings and preferences. This high degree of customization enables developers to tailor their coding environment to suit their needs and preferences.
8. **Integrated Terminal:** The integrated terminal within VS Code lets developers run commands and scripts directly within the editor, eliminating the need to switch between the code editor and a separate terminal window.
9. **Version Control:** Git integration is a core feature of VS Code, making it easy to manage version control, commit changes, and work with repositories without leaving the editor.
10. **Task Automation:** VS Code supports task automation through customizable tasks and build configurations, allowing developers to streamline common development tasks.
11. **Live Share:** This collaborative feature enables developers to work together on code in real-time, even if they are located in different parts of the world. It's a valuable feature for pair programming and remote collaboration.
12. **Accessibility:** VS Code is designed with accessibility in mind, making it usable for individuals with disabilities. It includes features like screen reader support and high-contrast themes.

In summary, Visual Studio Code is a versatile and highly extensible code editor that has gained immense popularity in the developer community. Its combination of performance, customization options, and a vast extensions ecosystem makes it an invaluable tool for programmers across the globe.

### <mark style="color:blue;">**How It Works**</mark>

<mark style="color:orange;">Visual Studio Code (VS Code) operates as a powerful and user-friendly code editor, enhancing the coding experience for developers across diverse programming languages and platforms. Its functionality and operation are rooted in the following key aspects:</mark>

1. **Installation and Launch:** To begin using VS Code, developers typically download and install it on their chosen operating system, such as Windows, macOS, or Linux. Once installed, launching the application is as simple as opening the executable file.
2. **User Interface:** VS Code presents a clean and intuitive user interface. The editor window serves as the primary workspace, where developers write and edit code. The interface includes menus, toolbars, and sidebars that provide access to various features and functionalities.
3. **Workspace and Projects:** Users can create and manage workspaces and projects within VS Code. A workspace is a collection of related folders and files, while a project is a specific configuration of a workspace. This organization helps developers structure their coding tasks effectively.
4. **File Management:** Developers can create, open, and edit files directly within VS Code. The editor supports a wide range of file types, including source code, configuration files, and documentation.
5. **Extensions:** A standout feature of VS Code is its extensibility through extensions. Developers can browse and install extensions from the Visual Studio Code Marketplace. These extensions enhance the editor's capabilities and offer support for specific programming languages, frameworks, and tools.
6. **Code Editing:** VS Code provides a feature-rich code editing experience. It includes syntax highlighting, code folding, auto-indentation, and smart code completion. Users can easily navigate code using features like "Go to Definition" and "Find All References."
7. **Integrated Terminal:** VS Code incorporates an integrated terminal that allows developers to run shell commands and scripts directly within the editor. This feature streamlines tasks like compiling code, running tests, and executing version control commands.
8. **Debugging:** Debugging is an integral part of the development process, and VS Code offers seamless integration with debugging tools. Developers can set breakpoints, inspect variables, and step through code to identify and resolve issues.
9. **Version Control:** Git integration is built into VS Code, enabling developers to manage version control operations from within the editor. Users can commit changes, view commit history, and work with Git repositories without leaving the application.
10. **Extensions Marketplace:** VS Code boasts a vast ecosystem of extensions that cater to various development needs. These extensions can add support for programming languages, integrate with cloud services, or enhance productivity with additional features.
11. **Customization:** VS Code places a strong emphasis on customization. Users can personalize their coding environment by selecting themes, configuring keybindings, and adjusting editor settings to suit their preferences.
12. **Live Share:** The "Live Share" feature enables real-time collaboration between developers working on the same codebase. It allows multiple users to edit and debug code together, even across geographical distances.
13. **Accessibility:** Accessibility features, such as screen reader support and high-contrast themes, make VS Code inclusive and accessible to users with disabilities.

In summary, Visual Studio Code is a versatile and extensible code editor that accommodates a wide range of programming languages and development tasks. Its user-friendly interface, robust feature set, and extensive extension ecosystem make it a preferred choice for developers seeking an efficient and customizable coding environment.

### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official VSCODE Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the <mark style="color:orange;">VSCODE</mark> application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the <mark style="color:orange;">VSCODE</mark> application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the <mark style="color:orange;">VSCODE</mark> webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed <mark style="color:orange;">VSCODE</mark> application and gained access to its features through a seamless and user-friendly process.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<mark style="color:orange;">VSCODE</mark>](https://hub.docker.com/r/linuxserver/openvscode-server)<mark style="background-color:yellow;">👈(click me,for the dockerhub image)</mark> |

| Application name                                                            |
| --------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: vs1(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">3000</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

| Install with Default                                                                                                                                        | Advanced                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">(select this if you want install with default settings if don't have environment value and working directory)</mark> | <mark style="background-color:yellow;">(select this if you want to go with advanced settings, where you select you own environment value and working directory)</mark> |

If you choose Advanced option:

| ENV VARIABLE                                                            |
| ----------------------------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> |

| WORKING DIR                                                                                                  |
| ------------------------------------------------------------------------------------------------------------ |
| <p><code>WORKDIR for the application.</code></p><p> <code>Eg:usr/src/yourAPP</code></p>                      |
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                                      |
| <p></p><pre class="language-bash"><code class="lang-bash">-v /path/to/appdata/config:/config \
</code></pre> |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to VSCODE Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`VSCODE`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `VSCODE`
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `3000`
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

           ```bash
           -v /path/to/appdata/config:/config \
           ```
6. <mark style="color:orange;">**Access Configuration**</mark>**:**
   * Choose between "Public" or "Private" access to the deployed application.
7. <mark style="color:orange;">**Installation**</mark>**:**
   * Click the "Install" button to initiate the deployment process.

By following these steps, you can effortlessly deploy an VSCODE instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-06 115254.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-06 115347.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-09-06 115423 (1).png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.



### <mark style="color:blue;">FAQ</mark>

**About vSCODE image we used.**

This is the official vSCODE image.

**Can I deploy my own vscode image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
