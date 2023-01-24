---
authors: ["inisialb"]
title: "Menjalankan MySQL/MariaDB Di Centos 7"
slug: menjalankan mysql di centos 7
description: Menjalankan dan membuat user remote MySQL/MariaDB di CentOS 7
date: 2023-01-23T20:57:13+07:00
tags : 
    - centos
    - mysql
categories : 
    - tutorial
    - linux
toc : false
---

## Menjalankan MariaDB/MySQL di CentOS 7

> Catatan : Dalam penginstalan CentOS 7 with GUI dan MariaDB Database Server sudah terinstall di dalamnya dengan Mysql/MariaDB `Server version: 5.5.60-MariaDB MariaDB Server`

1. Jalankan service MySQL

    ```
    $ systemctl enable mariadb

    $ systemctl start mariadb
    ```

2. Buat User Remote

    Jalan kan perintah `mysql` untuk masuk ke MySQL :

    ```
    $ mysql
    ```

    ![](https://imgur.com/3lyCKe3.png "Login MySQL")

    ```
    > create user 'root'@'%' identified by 'password';

    > grant all privileges on *.* to 'root'@'%' with grant option;

    > flush privileges;
    ```