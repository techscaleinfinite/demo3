# Wordpress Mysql

WordPress is a free and open-source content management system written in hypertext preprocessor language and paired with a MySQL or MariaDB database with supported HTTPS.

**➡️ Docker image of this application consists of following layers :**

```
'FROM ubuntu:14.04' Taking ubuntu:14.04 as the base image.

And updating and installing all the required softwares like 'mysql-server' 'mysql-client' 'nginx' for better performance 'php5-fpm' 'php5-mysql'.

And installing all the required softwares for Wordpress 'php5-curl' 'php5-gd' 'php5-intl'

Done configurations in required files like adding nginx keepalive_timeout and wordpress upload and post max file size.

Exposing 3306 and 80 ports on the container. 
```

#### Deploy Wordpress Mysql on Scaleinfinite

➡️ Go to create apps page and Search scaleinfinite/wpmysql on the search bar.

➡️ Click on install button.

➡️ Fill all the reqired feilds.

| PRODUCT NAME |
| ------------ |
| `Wpmysql`    |

`PROTOCOL`

| HTTP | TCP/UDP |
| ---- | ------- |
| `80` |         |

➡️ click on Advanced.

| ENV VARIABLE        | WHITELIST                                       | WORKING DIR                   |
| ------------------- | ----------------------------------------------- | ----------------------------- |
| `Give env variable` | `If you want to white list any ports list here` | `WORKDIR for the application` |

➡️ Click on the Install button.

➡️ You will be redirected to My Apps page, Here you can find all the applications you deployed.

➡️ Copy the wpmysql application Hostname without NodePort and search the Url.

➡️ Now you can see the wordpress language selection page.

➡️ After selecting language you will be directly redirected to site creation page and fill all the fields like site name and username and so on.

➡️ Then Login with that detials.

➡️ Then you will be redirected to the wordpress Admin dashboard.

### FAQ

**About Wordpress mysql image we used.**

This image is maintained by the scaleinfinite.

**Is Mysql is in the same container ?**

Yes, both WordPress and MySQL are inbuilt into the same container securely.

**Do the image secure to use ?**

The image is created and verified by the scaleinfinite. it is a 100% secure image.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.
