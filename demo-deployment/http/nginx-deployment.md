---
cover: ../../.gitbook/assets/NGINX-logo-rgb-large (1).png
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

# Nginx deployment

### <mark style="color:blue;">What's is Nginx?</mark>

Nginx is more than a web server; it's a multitool for your online presence:

* <mark style="color:orange;">**Web Server**</mark>**:** Delivers web content quickly and efficiently to users.
* <mark style="color:orange;">**Reverse Proxy**</mark>**:** Safeguards applications by managing external requests.
* <mark style="color:orange;">**Load Balancer**</mark>**:** Distributes traffic among multiple servers for optimal performance.
* <mark style="color:orange;">**Mail Proxy**</mark>**:** Routes emails effectively, improving email infrastructure.
* <mark style="color:orange;">**HTTP Cache**</mark>**:** Stores and serves frequently accessed resources for faster delivery.

### <mark style="color:blue;">**How It Works:**</mark>

Nginx's event-driven architecture handles multiple connections simultaneously, making it perfect for high-traffic scenarios. It's resource-efficient and enhances application performance, all while being open-source and free.

<mark style="color:blue;">Nginx: Streamline, secure, and supercharge your web operations</mark>

### <mark style="color:blue;">Steps And Procedure</mark>

* &#x20;<mark style="background-color:purple;">**This deployment uses the official Nginx Docker image.**</mark>
* &#x20;Go to create apps page and Search nginx on the search bar.
* &#x20;Click on install button.
* &#x20;Fill all the required fields.
* &#x20;click on Advanced.
* Click on the Install button.
* You will be redirected to My Apps page, Here you can find all the applications you deployed.
* &#x20;Copy the nginx application Hostname without NodePort and search the Url.
* &#x20;Now you can able to access the nginx webpage.

### <mark style="color:blue;">Installation</mark>

| Docker Image                               |
| ------------------------------------------ |
| [`nginx`](https://hub.docker.com/\_/nginx) |

`PROTOCOL`

| HTTP | TCP/UDP |
| ---- | ------- |
| `80` |         |

| ENV VARIABLE                                                            | WHITELIST                                       | WORKING DIR                                       |
| ----------------------------------------------------------------------- | ----------------------------------------------- | ------------------------------------------------- |
| <p><code>Give env variable.</code></p><p><code>Eg:key==value</code></p> | `If you want to white list any ports list here` | `WORKDIR for the application. Eg:usr/src/yourAPP` |



### <mark style="color:blue;">Visual Snapshots</mark>

<figure><img src="../../.gitbook/assets/myapps (3).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-12 152047.png" alt=""><figcaption></figcaption></figure>

### <mark style="color:blue;">FAQ</mark>

**About nginx image we used.**

This is the official nginx image.

**Can I deploy my own nginx image with modified configuration ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
