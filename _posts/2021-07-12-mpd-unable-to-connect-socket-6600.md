Assalamualaikum, saya mengalami masalah ketika installasi mpd & ncmpcpp berlangsung
<br> <b> port is already used 127.0.0.1:6600 </b>

Penyelesaian : 

untuk melihat PID apa yang sedang berjalan di socket tersebut  kita dapat mengeceknya menggunakan <b> netstat </b> yang dapat diinstall dengan nama paket <b> net-tools </b>di package manager apt
<br> <pre> sudo netstat -tnlp | grep 6600 </pre> </br> 
<img src="https://imgur.com/8NfpHSQ" alt=netstat-660">
