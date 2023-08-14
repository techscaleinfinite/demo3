# Wordpress Mysql

WordPress is a free and open-source content management system written in hypertext preprocessor language and paired with a MySQL or MariaDB database with supported HTTPS.

&#x20;**Docker image of this application consists of following layers :**

```
'FROM ubuntu:14.04' Taking ubuntu:14.04 as the base image.

And updating and installing all the required softwares like 'mysql-server' 'mysql-client' 'nginx' for better performance 'php5-fpm' 'php5-mysql'.

And installing all the required softwares for Wordpress 'php5-curl' 'php5-gd' 'php5-intl'

Done configurations in required files like adding nginx keepalive_timeout and wordpress upload and post max file size.

Exposing 3306 and 80 ports on the container. 
```

#### Deploy Wordpress Mysql on Scaleinfinite

* &#x20;Go to create apps page and Search scaleinfinite/wpmysql on the search bar.
* &#x20;Click on install button.
* Fill all the reqired feilds.

| PRODUCT NAME |
| ------------ |
| `Wpmysql`    |

`PROTOCOL`

| HTTP | TCP/UDP |
| ---- | ------- |
| `80` |         |

* &#x20;click on Advanced.

| ENV VARIABLE        | WHITELIST                                       | WORKING DIR                   |
| ------------------- | ----------------------------------------------- | ----------------------------- |
| `Give env variable` | `If you want to white list any ports list here` | `WORKDIR for the application` |

* &#x20;Click on the Install button.
* You will be redirected to My Apps page, Here you can find all the applications you deployed.



<figure><img src="../../.gitbook/assets/Screenshot 2023-08-12 153148.png" alt=""><figcaption></figcaption></figure>

* Copy the wpmysql application Hostname without NodePort and search the Url.
* Now you can see the wordpress language selection page.



<figure><img src="../../.gitbook/assets/Screenshot 2023-08-12 153222.png" alt=""><figcaption></figcaption></figure>

* After selecting language you will be directly redirected to site creation page and fill all the fields like site name and username and so on.



<figure><img src="../../.gitbook/assets/Screenshot 2023-08-12 153246.png" alt=""><figcaption></figcaption></figure>

➡️ Then Login with that detials.



<figure><img src="../../.gitbook/assets/Screenshot 2023-08-12 153317.png" alt=""><figcaption></figcaption></figure>

* Then you will be redirected to the WordPress Admin dashboard.



<figure><img src="../../.gitbook/assets/Screenshot 2023-08-12 153350.png" alt=""><figcaption></figcaption></figure>

### FAQ

**About Wordpress mysql image we used.**

This image is maintained by the scaleinfinite.

**Is Mysql is in the same container ?**

Yes, both WordPress and MySQL are inbuilt into the same container securely.

**Do the image secure to use ?**

The image is created and verified by the scaleinfinite. it is a 100% secure image.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.

#### [Join us](https://app.slack.com/client/T04QS32JX6E/C04QKEWE146)&#x20;
