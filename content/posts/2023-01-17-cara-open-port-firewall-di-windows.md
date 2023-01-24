---
authors : ["inisialb"]
title: "Membuka Port MySQL Di Windows Firewall"
description : "Cara Port MySQL Di Windows Firewall"
slug: "membuka port firewall di windows"
date: 2023-01-22T20:00:11+07:00
tags : 
    - port
    - mysql
categories : 
    - tutorial
    - windows
toc : true
---

Untuk membuka port di Windows 10, ikuti langkah-langkah berikut:

1. Klik tombol Start dan pilih Control Panel.
   
   ![Buka Port Firewall](https://i.imgur.com/njqQBov.png "Cari dan Pilih Control Panel")

2. Klik pada opsi "System and Security" dan pilih "Windows Firewall".

    ![Buka Port Firewall](https://i.imgur.com/2U4tbWW.png "Klik System and Security")
    ![Buka Port Firewall](https://i.imgur.com/WfxzrxR.png "Klik Windows Firewall")

3. Pada jendela Windows Firewall, klik pada opsi "Advanced settings" di sebelah kiri.

    ![Buka Port Firewall](https://i.imgur.com/kSIBcjn.png)

4. Pada jendela Inbound Rules, klik pada opsi "New Rule" di sebelah kanan.

    ![Buka Port Firewall](https://i.imgur.com/LBLQUqT.png)

5. Pada jendela New Rule Wizard, pilih opsi "Port" dan klik "Next".

    ![Buka Port Firewall](https://i.imgur.com/aaQVok1.png)

6. Pada jendela Protocol and Ports, pilih opsi "TCP" dan masukkan nomor port yang ingin dibuka. Kemudian klik "Next".

    ![Buka Port Firewall](https://i.imgur.com/JyATOTl.png)

7. Pada jendela Action, pilih opsi "Allow the connection" dan klik "Next".

    ![Buka Port Firewall](https://imgur.com/Lw483P5.png)

8. Pada jendela Profile, pilih profil jaringan yang ingin digunakan (contoh: Domain or Private, Public) dan klik "Next".

    ![Buka Port Firewall](https://imgur.com/0OASPXf.png)

9.  Pada jendela Name, beri nama pada aturan yang dibuat (contoh: Port 80) dan klik "Finish".

    ![Buka Port Firewall](https://imgur.com/4lgaxIT.png)

10. Selesai, port yang ditentukan telah dibuka dan dapat digunakan.
