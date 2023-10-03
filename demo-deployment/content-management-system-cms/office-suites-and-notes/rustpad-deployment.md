---
cover: ../../../.gitbook/assets/95412c80-c628-11eb-88e5-352f9edd9b96 (1).png
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

# 📓 Rustpad Deployment

### <mark style="color:blue;">What's rustpad?</mark>

<mark style="color:orange;">Rustpad: Where Real-Time Collaboration Meets Seamless Editing</mark>

<mark style="color:orange;">Imagine a text editor that's not just functional but also thrives on collaboration. Enter Rustpad, an open-source gem that's changing the way we work together on documents.</mark>

**Real-Time Editing**: Rustpad employs the operational transformation algorithm, ensuring that every edit is instantly synced across all collaborators' screens. It's like having a virtual writing party, where your ideas flow freely and effortlessly.

**Web-Based Simplicity**: No need for heavy installations or downloads. Simply share a link to your Rustpad document, and your peers can dive right into editing from their browsers. It's instant, accessible, and hassle-free.

<mark style="color:orange;">**Live Preview**</mark>: Watch your document transform in real time as you and your collaborators make changes. It's not just a text editor; it's a dynamic, living canvas for your ideas.

**Uninterrupted Workflow**: With Rustpad, there's no need to take turns or send files back and forth. Everyone edits simultaneously, ensuring a streamlined, interruption-free workflow.

<mark style="color:orange;">**Version Control**</mark><mark style="color:orange;">:</mark> Sometimes, you might need to revisit an earlier version of your document. Rustpad has your back, with built-in version control that allows you to roll back to previous states effortlessly.

Rustpad is where innovation meets simplicity. It's more than a text editor; it's a collaborative space for turning ideas into reality, in real time. Say goodbye to the delays of traditional document sharing and embrace the future of collaborative editing with Rustpad. Try it now and experience the seamless synergy of real-time collaboration.



### <mark style="color:blue;">**How It Works:**</mark>

<mark style="color:orange;">**How Rustpad Works: Crafting Collaborative Creativity**</mark>

Rustpad, the dynamic collaborative text editor, operates on the ingenious operational transformation algorithm, paving the way for a seamless editing experience. Here's the lowdown on how it all comes together:

**1. Share the Link**: Begin by sharing a Rustpad link with your fellow wordsmiths. This isn't just any link; it's your gateway to simultaneous collaboration. It's as simple as sending an invitation to a virtual writing soirée.

<mark style="color:orange;">**2. Real-Time Magic**</mark>: As you and your collaborators access the document from your respective browsers, Rustpad's operational transformation algorithm takes center stage. It ensures that every keystroke, every edit, is instantaneously reflected across all screens. It's like having a real-time conversation with your document.

**3. Live Preview**: Watch your document transform before your eyes. Rustpad's live preview feature gives you a dynamic, interactive canvas for your ideas. It's not just editing; it's a creative journey in motion.

**4. Uninterrupted Flow**: Gone are the days of taking turns or sending files back and forth. Rustpad allows everyone to edit simultaneously, harmonizing your efforts into an uninterrupted workflow. It's your personal symphony of ideas.

<mark style="color:orange;">**5. Version Control**</mark><mark style="color:orange;">:</mark> Need to revisit an earlier draft? Rustpad's built-in version control has you covered. Effortlessly roll back to previous states, ensuring that no brilliant idea is ever lost.

Rustpad isn't just a text editor; it's your creative cockpit, where innovation and collaboration take flight. Say farewell to the delays of traditional document sharing and embrace the future of real-time editing with Rustpad. It's where ideas flow freely, edits happen instantaneously, and your document transforms into a masterpiece right before your eyes. Try Rustpad today and experience the magic of collaborative creativity.

### <mark style="color:blue;">Steps And Procedure</mark>

*   <mark style="background-color:purple;">**This deployment utilizes the official rustpad Docker image. Here's a step-by-step guide to get you started:**</mark>

    1. Begin by navigating to the "Create Apps" page and use the search bar to find the [ekzhang/rustpad](https://hub.docker.com/r/ekzhang/rustpad)application.
    2. Click on the "Install" button to initiate the installation process.
    3. Fill in all the required fields with the necessary information.
    4. If you prefer, you can click on the "Advanced" option to access additional settings (this step is optional).
    5. After making your selections, press the "Install" button to proceed.
    6. Once the installation is complete, you'll be directed to the "My Apps" page, where you'll find a list of all the applications you've deployed.
    7. Copy the Hostname of the Rustpad application without the NodePort and paste it into your preferred browser's address bar.
    8. Voilà! You're now able to access the  Rustpad webpage and explore its content.

    By following these straightforward steps, you'll have successfully deployed the Rustpad application and gained access to its features through a seamless and user-friendly process.



### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                                                                                                                                        |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Rustpad](https://hub.docker.com/r/ekzhang/rustpad)[<mark style="background-color:yellow;">👈(</mark>](https://hub.docker.com/r/linuxserver/firefox)<mark style="background-color:yellow;">click me,for the dockerhub image)</mark> |

| Application name                                                             |
| ---------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: rust(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">3030</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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
| <mark style="color:red;">Here use ( use the path after   " :"  )</mark>                 |

<mark style="background-color:yellow;">`Access`</mark>

| Public                                      | Private                                      |
| ------------------------------------------- | -------------------------------------------- |
| (select this if you want to make it public) | (select this if you want to make it private) |

<mark style="color:purple;">**Step-by-Step Guide to RUSTPAD Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`rustpad`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `rustpad`
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP`
   * Port: `3030`
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

By following these steps, you can effortlessly deploy an Rustpad instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-08 124740.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-08 125028 (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-08 124804 (1).png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:orange;">Youtube Tutorial</mark>&#x20;

Check out our youtube video for more clarification.

### <mark style="color:blue;">FAQ</mark>

**About** Rustpad **image we used.**

This is the official Rustpad mage.

**Can I deploy my own media** Rustpad **with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;