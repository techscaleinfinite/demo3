# Drupal deployment

Drupal is a free and open-source web content management system written in PHP.

**➡️ This deployment uses the official Drupal Docker image.**

➡️ Go to create apps page and Search Drupal on the search bar.

➡️ Click on install button.

➡️ Fill all the reqired feilds.

| PRODUCT NAME |
| ------------ |
| `drupal`     |

`PROTOCOL`

| HTTP | TCP/UDP |
| ---- | ------- |
| `80` |         |

➡️ click on Advanced.

| ENV VARIABLE                                                                                                                 | WHITELIST                                       | WORKING DIR                   |
| ---------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------- | ----------------------------- |
| `You can set multiple ENV for database connection` `MYSQL_DATABASE, MYSQL_USER`, `MYSQL_PASSWORD`, and `MYSQL_ROOT_PASSWORD` | `If you want to white list any ports list here` | `WORKDIR for the application` |

➡️ Click on the Install button.

➡️ You will be redirected to My Apps page, Here you can find all the applications you deployed.

➡️ Copy the Drupal application Hostname without NodePort and search the Url.

➡️ Now you can access the Drupal login page.

➡️ Then you will be redirected to the Drupal dashboard page.

### FAQ

**About Drupal image we used.**

This is the official Drupal image.

**Is the Database inbuilted in the same image ?**

No, you need to add your database while you are login and setting your website.

**Can i deploy older version of drupal or my own modified drupal image ?**

Yes, you can simply deploy any version or modified image to our platform by linking your docker hub account to our platform.

**Are my data persistent ?**

For the free user there is no persistence, and for the premium user you can different type of persistence.
