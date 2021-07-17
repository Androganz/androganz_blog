---
layout : page 
title : how to setup neoivm with plugin 
---

Halo semua!,kali ini saya akan membagikan tutorial memasang neovim beserta Plugin nya.
Neovim 0.5 kini sudah di rilis menjadi stable bukan nightly lagi, namun di beberapa distribusi seperti debian 10 masih berada di versi 0.3.4 , sedangkan debian testing masih berada di versi 0.4.

<br>1.Install prerequisites  pada setiap distribusi masing masing</br> 
<br> <b>Debian 10</b> </br>
<pre> sudo apt-get install ninja-build gettext libtool libtool-bin autoconf automake cmake g++ pkg-config unzip</pre> 
<br> <b> Arch Linux </b> </br>
<pre> git clone https://github.com/neovim/neovim </pre> 

<br>2.Clone repository / source code berikut 
<pre> git clone https://github.com/neovim/neovim </pre> 

<br>3.Setelah selesai eksekusi perintah di bawah ini </br>
<pre> cd neovim && make -j4 </pre> 
Kalau teman teman mau yang versi stable bukan nightly lakukan perintah seperti di bawah 
<pre> <b> cd neovim && git checkout checkout stable && make </b>  
  #jika sudah selesai jalankan perintah 
  <b>sudo make install </b></pre>
<br> Proses building/make ini berlangsung lumayan lama , tergantung processor yang digunakan teman teman </br>

<br> 4.Proses pemasangan plugin pada neovim </br> 
Vim dan neovim mempunyai banyak plugin yang bisa di install,dan karena banyak nya plugin tersebut kita membutuhkan sebuah plugin manager untuk memanajemen plugin yang dipakai misal plugin tersebut mau di update, dihapus,dsb.salah satunya Vim-plug mudah digunakan baik saat installasi maupun penggunaanya . </br>

<br> Pertama kita wajib mempunyai file vimrc, kalau misal belum ada pasang vim kemudian copy file berikut: 





