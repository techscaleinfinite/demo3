---
description: For Private access
---

# My Account Page

1. N**avigate to the Create App Page**: To begin the deployment process, head over to our user-friendly Create App page.
2. **Search for Your Desired App**: In the search bar, type the name of the app you want to deploy. Our platform offers a wide range of pre-configured apps to choose from.
3. **Select Your Chosen App**: Once you've found the app you want, click on it to select it.

Then follow these steps:

<mark style="color:purple;">**Step-by-Step Guide to APP Deployment**</mark>

1. <mark style="color:blue;">**Docker Image Selection**</mark>**:**
   * <mark style="color:orange;">Docker Image Name:</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`XYZ`</mark>
2. <mark style="color:orange;">**Application Details**</mark>**:**
   * Application Name: `XYZ`
   * Resource Allocation: Set the desired resource allocation from 0-100%.
3. <mark style="color:orange;">**Protocol Configuration**</mark>**:**
   * Protocol: `HTTP/TCP`
   * Port: `GIVE PORT NUMBER EG:80,443 etc`
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

**Private Access:**

<mark style="color:orange;">When you choose "Private" access for your deployed application, it means that the application will not be publicly accessible over the internet. Instead, it will be accessible only within a restricted and controlled network environment</mark>. Here's what this entails:

1. **Limited Access:** With private access, the application will typically be available only to specific users or systems within your organization's network. It won't be accessible to the general public or external internet users.
2. **Enhanced Security:** Private access is often used for applications that contain sensitive or confidential data. By restricting access to a private network, you add an extra layer of security, reducing the exposure to potential security threats from the internet.
3. **Internal Use:** Private deployments are common for applications used exclusively by employees, contractors, or partners within a company. These applications might include internal tools, databases, or development environments.
4. **VPN or Direct Network Access:** To access a privately deployed application, users typically need to connect to the organization's network via a Virtual Private Network (VPN) or other secure methods. This ensures that they are within the trusted network perimeter.
5. **Compliance and Regulation:** Private access is often chosen to comply with data protection regulations, industry standards, or company policies that require strict control over data access and handling.
6. **Isolation:** Private deployments can also help isolate applications from external threats, reducing the risk of attacks and vulnerabilities.



<mark style="color:orange;">**Installation**</mark>**:**

* Click the "Install" button to initiate the deployment process.

In summary, selecting "Private" access during application deployment is a security and access control measure. It restricts the application's accessibility to a defined and trusted network environment, enhancing data protection and control. This option is particularly useful for applications that require strict confidentiality, limited access, or compliance with security standards.

By following these steps, you can effortlessly deploy an App instance with your chosen configurations. This enables you to tailor the environment to match your application's requirements and specifications. Whether opting for the default installation or delving into advanced settings, our platform ensures a seamless deployment experience while providing you the flexibility to customize according to your needs.

\
