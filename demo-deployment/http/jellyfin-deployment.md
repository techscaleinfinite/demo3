---
cover: ../../.gitbook/assets/download (1).png
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

# Jellyfin Deployment

### <mark style="color:blue;">What's Jellyfin?</mark>

Jellyfin is a versatile, open-source media server software designed to help users organize, manage, and stream their personal media collection, including music, videos, and pictures, across a range of devices.

**Key Points:**

1. <mark style="color:orange;">**Open-Source Media Server**</mark>**:** Jellyfin is freely accessible, providing a platform to organize and stream personal media.
2. **Media Variety:** It supports various types of media, from music tracks to videos and images.
3. <mark style="color:orange;">**Device Compatibility**</mark>**:** Jellyfin streams content to a wide array of devices, ensuring seamless access.
4. **Customization:** Tailor your media server's interface and functionality to suit your preferences.
5. <mark style="color:orange;">**User Privacy**</mark>**:** Your media collection remains private as it's self-hosted, with no external sharing.

### <mark style="color:blue;">**Working in Brief:**</mark>

1. **Media Organization:** Jellyfin catalogues your media library, allowing you to arrange content by type, genre, or artist.
2. <mark style="color:orange;">**Streaming Capability**</mark>**:** Upon request, Jellyfin streams media to connected devices over a local network or the internet.
3. **User Authentication:** Users log in to their Jellyfin accounts to access their personalized media libraries.
4. <mark style="color:orange;">**Transcoding & Formats**</mark>**:** Jellyfin adapts media formats for compatibility with different devices.
5. **Remote Access:** Enjoy your media on-the-go by accessing your Jellyfin server from external locations.

Jellyfin simplifies media management, offering a self-hosted solution for streaming your favorite content across various devices. Its open-source nature empowers customization and ensures that your media remains private and secure.

### <mark style="color:blue;">Steps And Procedure</mark>

* &#x20;<mark style="background-color:yellow;">**This deployment uses the linuxserver/jellyfin Docker image**</mark>**.**
* &#x20;Go to create apps page and Search linuxserver/jellyfin on the search bar.
* &#x20;Click on install button.
* &#x20;Fill all the required fields.
* click on Advanced.
* Default Installation is enough for Jellyfin to be up and running. Click install
* You will be redirected to My Apps page, Here you can find all the applications you deployed.
* &#x20;Copy the Jellyfin application Hostname without NodePort and search the Url.
* &#x20;Now you will access the application. And start setting up the application.
* &#x20;Now Follow the on screen instructions and setup your account
* &#x20;We’ll add media files using ftp
* &#x20;Goto SFTP section in right-side bar menu and click 'Reinitilze password'
* &#x20;You will get credentials to login to your sftp storage. SFTP storage can be accessed using various tools, example:- Filezilla
* Select HDD to Server
* &#x20;Make sure you have provided right From and To file paths
* &#x20;Add the uploaded media files into the jellyfin using its web interface

### <mark style="color:blue;">Installation</mark>

| Docker Image                                             |
| -------------------------------------------------------- |
| [`Jellyfin`](https://hub.docker.com/r/jellyfin/jellyfin) |

`PROTOCOL`

| HTTP   | TCP/UDP |
| ------ | ------- |
| `8096` |         |

| ENV VARIABLE                                                            | WHITELIST                                       | WORKING DIR                                       |
| ----------------------------------------------------------------------- | ----------------------------------------------- | ------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> | `If you want to white list any ports list here` | `WORKDIR for the application. Eg:usr/src/yourAPP` |

### <mark style="color:blue;">Visual Snapshots</mark>

<figure><img src="../../.gitbook/assets/my-apps.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/select-hdd-to-server.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/sftp-upload.png" alt=""><figcaption></figcaption></figure>

### <mark style="color:blue;">FAQ</mark>

**About Jellyfin image we used.**

This is the official linuxserver/jellyfin image.

**Are there any restrictions on adding data sources ?**

you can add any data source that Jellyfin supports.

**Can i deploy older version of Jellyfin or my own modified Jellyfin image ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
