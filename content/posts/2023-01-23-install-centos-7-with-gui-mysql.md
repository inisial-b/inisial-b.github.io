---
authors: ["inisialb"]
title: "Install Server CentOS 7 With GUI"
slug: "install server centos 7 with gui"
description : Install Server CentOS 7 With GUI dan MySQL.
date: 2023-01-23T14:35:44+07:00
tags : 
    - centos
    - mysql
categories : 
    - tutorial
    - linux
toc : true
---

1. Boot dari DVD atau USB instalasi CentOS 7. Pilih "Install CentOS 7" dari menu boot.

    !["Install Server CentOS 7 With GUI"](https://ik.imagekit.io/inisialb/install-server-centos-7-with-gui/KmeQJiO.png "Pilih Install CentOS 7")

2. Pilih bahasa yang akan digunakan selama proses instalasi. Pilih Bahasa dan klik "Continue".

    !["Install Server CentOS 7 With GUI"](https://ik.imagekit.io/inisialb/install-server-centos-7-with-gui/h4QdOUd.png "Pilih Bahasa")

3. Ubah Date & Time menjadi `Asia/Jakarta`

4. Pada "Software Selection" pilih "Server with GUI" dan "MariaDB Database Server". Klik "Done".

    !["Install Server CentOS 7 With GUI"](https://ik.imagekit.io/inisialb/install-server-centos-7-with-gui/KJ23aDM.png)

5. Pada "Installation Destination" pilih "Hard Disk" dan pilih "I will configure partitioning". Klik "Done".

    !["Install Server CentOS 7 With GUI"](https://ik.imagekit.io/inisialb/install-server-centos-7-with-gui/hkFCpCy.png)

    Konfirmasi klik "Accept Changes"

    !["Install Server CentOS 7 With GUI"](https://ik.imagekit.io/inisialb/install-server-centos-7-with-gui/gJVO4yX.png?ik-sdk-version=javascript-1.4.3&updatedAt=1674549145150)

    Membuat partisi ada 3 partisi yang dibuat `boot`, `swap` dan `root`, Klik tanda ( + ) untuk membuat partisi

    !["Install Server CentOS 7 With GUI"](https://ik.imagekit.io/inisialb/install-server-centos-7-with-gui/BNDDl0X.png?ik-sdk-version=javascript-1.4.3&updatedAt=1674549143979)

    > Catatan : Umumnya partisi `"/"` `root` kapasitasnya di maksimalkan

6. Setelah semuanya sudah dipilih, klik "Begin Instalation"

    !["Install Server CentOS 7 With GUI"](https://ik.imagekit.io/inisialb/install-server-centos-7-with-gui/QloDBDq.png?ik-sdk-version=javascript-1.4.3&updatedAt=1674549147512)

7. Setting "Root Password" dan "User Creation", Lalu tunggu sampai proses instalasi selesai.

    !["Install Server CentOS 7 With GUI"](https://ik.imagekit.io/inisialb/install-server-centos-7-with-gui/Q8vUGdm.png)

8. Proses selesai, Klik "Reboot" untuk menyelesaikan instalasi.

    !["Install Server CentOS 7 With GUI"](https://ik.imagekit.io/inisialb/install-server-centos-7-with-gui/64COTZ9.png)

9. Selamat, sistem operasi CentOS 7 dengan GUI telah terinstal dengan sukses. Selamat menggunakan!

    !["Install Server CentOS 7 With GUI"](https://ik.imagekit.io/inisialb/install-server-centos-7-with-gui/f5oHkuy.png)
