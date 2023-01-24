---
title: "Install Ngrok Di Centos 7"
slug: install ngrok di centos 7
date: 2023-01-24T08:24:23+07:00
description : Remote Database dari lokasi lain melalui internet di centos 7.
tags : 
    - tunneling
    - mysql
categories : 
    - tutorial
    - linux
toc : false
---

## Aktifkan Snapd

1. Tambahkan Repositori EPEL dengan perintah berikut:

    ```
    $ sudo yum install epel-release
    ```

2. Install Snap

    ```
    $ sudo yum install snapd
    ```

3. Aktifkan `snap socket`

    ```
    $ sudo systemctl enable --now snapd.socket
    ```

4. Buat symbolic link 
   
   ```
   $ sudo ln -s /var/lib/snapd/snap /snap
   ```

## Install Ngrok

5. Install ngrok
   
   ```
   $ sudo snap install ngrok
   ```

6. Tambahkan authtoken, dapatkan token dengan login di situs [`ngrok`](https://ngrok.com)
   
   ```
   $ ngrok config add-authtoken <token>
   ```

7. Jalankan tunnel `tcp 3306` port 3306 adalah port umum MySQL

    ```
    $ ngrok tcp 3306
    ```
8. Anda akan melihat alamat URL yang digunakan untuk mengakses server Anda secara remote.

    ```terminal
    Session Status                online
    Account                       inisialb (Plan: Free)
    Update                        update available (version 3.1.1, Ctrl-U to update)
    Version                       3.1.0
    Region                        Asia Pacific (ap)
    Latency                       30ms
    Web Interface                 http://127.0.0.1:4040
    Forwarding                    tcp://0.tcp.ap.ngrok.io:16275 -> localhost:3306

    Connections                   ttl     opn     rt1     rt5     p50     p90
                                  0       0       0.00    0.00    0.00    0.00
    ```