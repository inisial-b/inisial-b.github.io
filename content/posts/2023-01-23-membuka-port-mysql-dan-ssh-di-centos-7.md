---
authors: ["inisialb"]
title: "Membuka Port MySQL dan SSH di CentOS 7"
slug: "Membuka Port MySQL dan SSH di CentOS 7"
description : Membuka Port MySQL dan SSH di CentOS 7
date: 2023-01-23T20:37:11+07:00
tags : 
    - centos
    - port
    - firewall
    - mysql
    - ssh
categories : 
    - tutorial
    - linux
toc : false
---

1. Cek status firewall

    ```
    systemctl status firewalld
    ```

    Output :
    ![Output Status Firewall](https://imgur.com/uFdGYiw.png "Output status Firewall")

2. Buka Port MySQL dan SSH

    MySQL :
    ```
    firewall-cmd –-permanent -–zone=public -–add-port=3306/tcp
    ```

    SSH :

    ```
    firewall-cmd –-permanent -–zone=public -–add-port=22/tcp
    ```
3. Restart service Firewallld

    ```
    systemctl restart firewalld
    ```