---
author : Inisial B
title : Install Ngrok
date : 2023-01-20T13:16:43+07:00
description : Remote Database dari lokasi lain melalui internet.
tags : [
    tunneling,
    mysql,
    windows,
]
categories : [
    tutorial
]
toc : true
---

## Apa itu Ngrok?
Ngrok adalah perangkat lunak yang memungkinkan Anda untuk me-remote jaringan lokal Anda dan mengaksesnya dari mana saja melalui internet. Ini sangat berguna saat Anda ingin mengakses aplikasi atau server yang dijalankan di komputer Anda dari lokasi lain, seperti dari perangkat mobile atau komputer lainnya.

## Setting Ngrok di Windows
Untuk mengatur ngrok dan me-remote TCP port 3306 pada Windows 10, ikuti langkah-langkah berikut:

1. Download ngrok dari situs resmi [`ngrok`](https://ngrok.com/download).

2. Ekstrak file yang telah diunduh ke direktori yang Anda inginkan.

3. Buka Command Prompt dan arahkan ke direktori ngrok yang telah Anda ekstrak.

4. Jalankan perintah `ngrok.exe tcp 3306` untuk menjalankan ngrok dan me-remote port 3306.

    ```terminal
    $ ngrok.exe tcp 3306
    ```

    >Catatan: Port `3306` adalah port tunnel untuk remote MySQL. Jika port tunnelingnya berbeda, maka silakan sesuaikan dengan port tersebut.

5. Anda akan melihat alamat URL yang digunakan untuk mengakses server Anda secara remote.

    ```terminal
    Session Status                online
    Account                       inisialb (Plan: Free)
    Update                        update available (version 3.1.1, Ctrl-U to update)
    Version                       3.1.0
    Region                        Asia Pacific (ap)
    Latency                       30ms
    Web Interface                 http://127.0.0.1:4040
    Forwarding                    tcp://0.tcp.ap.ngrok.io:17568 -> localhost:3306

    Connections                   ttl     opn     rt1     rt5     p50     p90
                                  0       0       0.00    0.00    0.00    0.00
    ```
6. Pastikan firewall anda memperbolehkan koneksi ke port 3306.