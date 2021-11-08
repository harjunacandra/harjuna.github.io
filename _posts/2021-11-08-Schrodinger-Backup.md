---
published: false
---
---
published: true
title: Schrodinger Backup
updated: '2021-11-08 18:13'
---

_**The condition of any backup is unknown until a restore is attempted.**_

Schrodinger Backup, Istilah ini sering muncul makbedunduk pada diguyonkan oleh account2 tech ditwitter dan instagram. Yaaa pada Waktu baca itu saya juga hanya mesam mesem karena memang lucu kalau sudah susah-susah backup tapi ternyata  kagak bisa digunakan, Sampai saat itu saya mengalaminya sendiri

Alkisah.

Tahun 2019-2020 adalah tahun kejayaan saya melakukan homelabing. Waktu itu saya berhasil melakukan implementasi homelab  seperti yang ada di kantor-kantor kecil, dari menggunakan LDAP untuk autentikasi, UPS untuk backup power, Router, FW, VPS, Site to site VPN, dsb. Availibility adalah hal yang saya yang agung-agungkan atau mungkin udah saya matur sembah sujud di Lab saya. Koneksi saya redundant, menggunakan kabel dan broadband. UPS harus servergrade agar server bisa tetap beroperasi lancar walaupun mati listrik. servicepun sebisa mungkin dibuat HA agar apabila satu down masih bisa digunakan. 
Hanya 1 hal yang waktu itu masih belum bisa dilakukan karena kendala biaya, mirroring ZFS menggunakan NAS (sekarang juga masih terkendala). 

Dengan hampir sempurnanya homelab saya, sayapun mulai berpikir, sebenarnya apa fungsi dari homelab saya ini. Karena kalau memang dilihat oleh orang lain, homelab saya ini tidak ada fungsinya sama sekali dan hanya membuang-buang uang saya. Saya pernah mencoba untuk mengusulkan untuk membuat home automation dan cctv tapi ditolak mentah-mentah karena masih ngontrak. 

Akhirnya, untung Tak dapat Diraih, malang Tak Dapat Ditolak, awal 2021 saya harus melakukan purge semua homelab saya, baik dari sisi cloud maupun dari on premise. Saya sudah legowo dengan keputusan ini karena memang keadaan yang memaksa saya. Ya Sudahlah, toh saya juga sudah melakukan incremental backup perminggu sejak server dideploy dan saya juga sudah melakukan 3-2-1 backup. Jadi, kalau terjadi apa-apa dengan salah satu backup saya, saya masih bisa melakukan restore dari tempat lainnya.

hampir Setaun berlalu...

Hari ini, tanggal 8 Nov 2021 saya bermaksud memulai kembali projek homelab saya dengan tujuan agar skill saya tidak usang dan karatan. Waktu pertama kali saya mencoba melakukan konfigurasi FW dan Server, saya lupa semua hal tentang cara konfigurasi perangkat2 ini. Yang saya ingat hanya cara buat install aplikasi dan update server ahahaha. 

Yoweslah, saya akhirnya mencoba melakukan restore backup yang sudah saya keep selama hampir satu tahun. Ternyata file backup ini saya enkrip dan saya juga lupa gimana cara dekripnya. Skipskip, alhamdulillah, setelah dioprek2 dan membaca tutorial, file backup telah berhasil didekrip. Semua file backup tinggal diektrak agar harjuna homelabs bisa berjaya kembali. Daaaaan, duaar,  ternyata.... filenya corrupt dan saya gak bisa bisa restore semua config dan semua file backup corrupt termasuk backup 3-2-1 dan ternyata yang salah cara backup saya dan dan dan dan dan masih banyak "dan" lagi yang isinya penuh penyesalan. 

Apalah artinya backup incremental dan metode 3-2-1 kalau ternyata metode backupnya yang bikin corrupt.

Jemb** memang.