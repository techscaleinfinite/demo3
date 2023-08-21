---
cover: ../../.gitbook/assets/grafana3182.jpg
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

# Grafana deployment

### <mark style="color:blue;">What's Grafana?</mark>

Grafana is a versatile, open-source analytics and interactive visualization web application. It empowers users to create compelling charts, graphs, and alerts by connecting to supported data sources.

**Key Points:**

1. <mark style="color:orange;">**Multi-Platform Analytics**</mark>**:** Grafana is available across various platforms, making data analysis accessible.
2. **Open-Source:** It's freely available, fostering collaboration and customization.
3. <mark style="color:orange;">**Interactive Visualization**</mark>**:** Grafana offers dynamic charts, graphs, and dashboards to illustrate data trends.
4. **Data Source Connectivity:** It connects to various data sources, like databases, APIs, and cloud services.
5. <mark style="color:orange;">**Alerting System:**</mark> Grafana can trigger alerts based on preset conditions to notify users of changes.

### <mark style="color:blue;">**Working in Brief:**</mark>

1. **Data Source Connection:** Grafana connects to your chosen data source, whether it's a database or cloud service.
2. <mark style="color:orange;">**Dashboard Creation**</mark>**:** Users design dashboards by selecting data metrics, visualizations, and layout.
3. <mark style="color:orange;">**Interactive Visuals**</mark>**:** Charts and graphs respond in real-time to user interactions, aiding analysis.
4. **Alert Configuration:** Set conditions for alerts to notify users when specific thresholds are met.
5. <mark style="color:orange;">**Real-Time Insights**</mark>**:** Grafana visualizes data trends, helping users grasp patterns and make informed decisions.

Grafana transforms raw data into visually engaging insights, enhancing data-driven decision-making. Its open-source nature and compatibility with multiple data sources make it an invaluable tool for monitoring and understanding complex datasets.

### <mark style="color:blue;">Steps And Procedure</mark>&#x20;

* &#x20;<mark style="background-color:yellow;">**This deployment uses the official Grafana Docker image.**</mark>
* &#x20;Go to create apps page and Search <mark style="color:orange;">grafana</mark> on the search bar.
* &#x20;Click on install button.
* &#x20;Fill all the required fields.
* &#x20;click on Advanced.
* &#x20;Click on the Install button.
* &#x20;You will be redirected to My Apps page, Here you can find all the applications you deployed.
* &#x20;Copy the grafana application Hostname without NodePort and search the Url.
* &#x20;Now you will access the application. And you need to login to grafana.
* &#x20;Default Username and Password for grafana is admin.
* &#x20;After you will be required to add datasources and create dashboards to visualize your data.    `ADD DATASOURCE`
* &#x20;Now you can create the dashboard and select the data source to visualize the data you need.

### <mark style="color:blue;">Installation</mark>

| Docker Image                                                                                                    |
| --------------------------------------------------------------------------------------------------------------- |
| [`grafana`](https://hub.docker.com/r/grafana/grafana)<mark style="background-color:yellow;">👈(click me)</mark> |

| Application name                                                                 |
| -------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">Eg: grafana1(you can put any name)</mark> |

| Resource Allocation                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <mark style="background-color:yellow;">0-100%(</mark><mark style="color:orange;">10 % of your allocated resources (CPU, RAM) will be used for this application.)</mark> |

<mark style="background-color:yellow;">`PROTOCOL`</mark>

<table><thead><tr><th width="417">Protocol</th><th>Protocol Value</th></tr></thead><tbody><tr><td><mark style="background-color:yellow;">Http</mark></td><td><mark style="color:orange;">80/3000</mark></td></tr><tr><td><mark style="background-color:yellow;">Tcp</mark></td><td>-</td></tr></tbody></table>

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

<mark style="color:purple;">**Step-by-Step Guide to Grafana Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`grafana`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `grafana1`
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

By following these steps, you can effortlessly deploy an GRAFANA instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

### <mark style="color:blue;">Visual Snapshots</mark>



<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 163652.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-21 164123.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/datasources (2).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/grafana-dashboard (1).png" alt=""><figcaption></figcaption></figure>

</div>

### <mark style="color:blue;">FAQ</mark>

**About grafana image we used.**

This is the official grafana image.

**Are there any restrictions on adding data sources ?**

you can add any data source that grafana supports.

**Can i deploy older version of grafana or my own modified grafana image ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

### Join us

Stay informed and engaged with our project's latest developments and support on [Slack](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146). Join us today to connect, collaborate, and keep the momentum going!&#x20;
