# Concepts

### <mark style="color:orange;">Some Key Concepts</mark>

<mark style="color:orange;">**App Redeployment and Data Persistence in Kubernetes:**</mark> When you redeploy an application in Kubernetes, the default behavior is to replace the existing pods with new ones containing the updated application. This process involves stopping the old pods and starting new ones. However, there's an important consideration regarding data persistence.

By default, when you redeploy an application, the data stored within the application's container is lost, as the old containers are terminated. But don't worry, you can take steps to make your application's data persistent.

<mark style="color:orange;">**Persistent Storage with Kubernetes:**</mark> Kubernetes offers solutions for persistent storage. You can configure your application to use external storage options like Persistent Volume Claims (PVCs) or StatefulSets. These mechanisms allow you to store data outside of the application containers. The benefit? Even if the application pods are replaced or redeployed, your data remains secure and accessible.

<mark style="color:orange;">**"Go" Button for Data Persistence:**</mark> Imagine a "Go" button on our platform that empowers you to make your app's data persistent. Clicking this button could prompt Kubernetes to associate your app with a Persistent Volume Claim. The result? Your data stays safe and sound, even if you decide to redeploy the app.

<mark style="color:orange;">**Upgrades, Port Changes, and Kubernetes:**</mark> When you upgrade your application or modify its configuration (such as changing the port), Kubernetes is here to help. It seamlessly manages this process, ensuring minimal downtime by gradually replacing the old pods with new ones.

<mark style="color:orange;">**Temporary vs. Persistent Storage:**</mark> Temporary storage, like RAM, can hold data only while the application is running. Once the app stops or restarts, this data disappears. To enhance data resilience, consider persistent storage. It involves storing data in a Persistent Volume, which could be on a hard disk, network storage, or even a cloud-based solution. This way, your data remains intact even when your application goes through changes or upgrades.

In summary, Kubernetes offers you control over data persistence during application redeployment. With persistent storage solutions and the "Go" button, you can ensure that your valuable data stays safe and accessible throughout your application's lifecycle.

\
