# Drupal deployment

Drupal is a free and open-source web content management system written in PHP.

* &#x20;**This deployment uses the official Drupal Docker image.**
* &#x20;Go to create apps page and Search Drupal on the search bar.
* Click on install button.
* &#x20;Fill all the reqired feilds.

| PRODUCT NAME |
| ------------ |
| `drupal`     |

`PROTOCOL`

| HTTP | TCP/UDP |
| ---- | ------- |
| `80` |         |

* &#x20;click on Advanced.

| ENV VARIABLE                                                                                                                 | WHITELIST                                       | WORKING DIR                   |
| ---------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------- | ----------------------------- |
| `You can set multiple ENV for database connection` `MYSQL_DATABASE, MYSQL_USER`, `MYSQL_PASSWORD`, and `MYSQL_ROOT_PASSWORD` | `If you want to white list any ports list here` | `WORKDIR for the application` |

* &#x20;Click on the Install button.
* &#x20;You will be redirected to My Apps page, Here you can find all the applications you deployed.



<figure><img src="../../.gitbook/assets/Screenshot 2023-08-12 153921.png" alt=""><figcaption></figcaption></figure>

* &#x20;Copy the Drupal application Hostname without NodePort and search the Url.



<figure><img src="../../.gitbook/assets/Screenshot 2023-08-12 154027.png" alt=""><figcaption></figcaption></figure>

* &#x20;Now you can access the Drupal login page.
* &#x20;Then you will be redirected to the Drupal dashboard page.



<figure><img src="../../.gitbook/assets/Screenshot 2023-08-12 154105.png" alt=""><figcaption></figcaption></figure>

### FAQ

**About Drupal image we used.**

This is the official Drupal image.

**Is the Database inbuilted in the same image ?**

No, you need to add your database while you are login and setting your website.

**Can i deploy older version of drupal or my own modified drupal image ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.
