---
published: true
title: Schrodinger Backup
updated: '2021-11-08 18:13'
---

_**The condition of any backup is unknown until a restore is attempted.**_

Schrodinger Backup, Istilah ini sering muncul mak-_bedunduk_ dan di-_guyon_-kan oleh _account2_ _tech_ di Twitter dan Instagram. Yaaa pada waktu baca itu, saya juga hanya _mesam-mesem_ karena memang lucu aja. Apalagi kalau sudah susah-susah backup tapi ternyata kagak bisa digunakan. Sampai saat itu saya mengalaminya sendiri...

Alkisah.

Tahun 2019-2020 adalah tahun kejayaan saya melakukan _homelabing_. Waktu itu, saya berhasil melakukanimplementasi _homelab_ seperti yang ada di kantor-kantor kecil. Dari menggunakan LDAP untuk autentikasi, UPS untuk backup power, Router, FW, VPS, hingga Site to site VPN menggunakan OPENVPN. _Availability_ adalah hal yang saya yang agung-agungkan atau mungkin saya sudah _matur sembah sujud_ di Lab saya. Koneksi saya _redundant_, menggunakan kabel dan _broadband_. UPS harus _servergrade_ agar server bisa tetap beroperasi lancar walaupun mati listrik. _service_-pun sebisa mungkin dibuat HA agar apabila satu _down_ masih bisa digunakan. 
Hanya 1 hal yang waktu itu masih belum bisa dilakukan karena kendala biaya, _mirroring_ ZFS menggunakan NAS (sekarang juga masih terkendala). 

Dengan hampir sempurnanya _homelab_ saya, sayapun mulai berpikir, sebenarnya apa fungsi dari _homelab_ saya ini? Karena kalau memang dilihat oleh orang lain, _homelab_ saya ini tidak ada fungsinya sama sekali dan hanya membuang-buang uang. Saya pernah mencoba untuk mengusulkan untuk membuat _home_ _automation_ dan CCTV tapi ditolak mentah-mentah karena masih ngontrak. 

Pada akhirnya, untung Tak dapat Diraih, malang Tak Dapat Ditolak. Awal 2021 saya harus melakukan _purge_ semua homelab saya, baik dari sisi _cloud_ maupun dari _on premise_. Saya sudah _legowo_ dengan keputusan ini karena memang keadaan yang memaksa. Ya Sudahlah, toh saya juga sudah melakukan _incremental_ _backup_ perminggu sejak server di-_deploy_. Saya juga sudah melakukan 3-2-1 _backup_ pada server dan _storage_. Jadi, kalau terjadi apa-apa dengan salah satu _backup_ saya, saya masih bisa melakukan _restore_ dari tempat lainnya.

hampir Setaun berlalu...

Hari ini, tanggal 8 Nov 2021 saya bermaksud memulai kembali projek _homelab_ saya dengan tujuan agar skill saya tidak usang dan karatan. Waktu pertama kali saya mencoba melakukan konfigurasi FW dan Server, saya lupa semua hal tentang cara konfigurasi perangkat2 ini. Yang saya ingat hanya cara buat _install_ aplikasi dan _update_ server ahahaha. 

> apt get update

Yoweslah, saya akhirnya mencoba melakukan _restore backup_ yang sudah saya _keep_ selama hampir satu tahun. Ternyata _file_ _backup_ ini saya enkrip dan saya juga lupa gimana cara dekripnya. Skipskip, Alhamdulillah, setelah dioprek-oprel dan membaca _tutorial_, _file backup_ telah berhasil didekrip. Semua _file backup_ tinggal diekstrak agar Harjuna Homelabs bisa berjaya kembali. Daaaaan, duaar,  ternyata.... filenya _corrupt_ dan saya gak bisa bisa _restore_ semua _config_ dan semua file _backup corrupt_ termasuk _backup_ 3-2-1 dan ternyata yang salah cara _backup_ saya dan dan dan dan dan masih banyak "dan" lagi yang isinya penuh penyesalan. 

Apalah artinya _backup_ _incremental_ dan metode 3-2-1 kalau ternyata metode backupnya yang bikin corrupt.

Jemb** memang.
