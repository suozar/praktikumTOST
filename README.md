## Pengertian ODK

Open Data Kit (ODK) is a free and open-source set of tools which help organizations author, field, and manage mobile data collection solutions.

Type Form adalah Surat Keterangan Lulus Ujian Tugas Akhir

##Prerequisite

 1. Java JDK
 2. Apache Tomcat 6.00 or 7.00
 3. MySQL 5.3+ or MariaDB

##Installation

 1. Download ODK Aggregate Installer.
 2. Install dengan mengikuti petunjuk yang ada di Installer.
Kemudian buka Readme.html yang ada dalam folder tujuan Installer
 3. Masukan syntax yang berada pada file create_db_and_user.sql kedalam database yang digunakan.
 4. Copy file ODKAggregate.war pada folder instalasi ke dalam webapps di tomcat
 5. Folder baru dalam webapps akan dibuat otomatis sama dengan isi ODKAggregate.war
 6. Masukan database connect .jar kedalam folder lib di dalam tomcat servernya, dalam kasus ini mysql-connector-java-5.1.38.jar
 7. Coba masuk kedalam alamat host tomcat server ODK. example: //localhost:8080/ODKAggregate/

----

###Create Form

    Buat form secara online menggunakan build.opendatakit.com
    Untuk contoh ada di folder from pada repo ini form/.....

###Upload form to ODKAggregate Server

    1. Loginlah kedalam user yang dibuat pada proses installasi.

    2. note:default password adalah aggregate.

    3. Upload pada menu form management.

###Collect data form ODK Connect on Android

   1. masuk pada play store, dan cari ODK Connect.
   2. kemudian install seperti biasa.
    > note:ODK Connect juga tersedia pada website opendatakit.com.

   3. kemudian buka applikasinya dan setting server sesuai dengan host yang disetting saat installasi.
   4. masuk kemenu Get Form, tunggu hingga selesai, kembali ke menu utama.
   5. kemudian masuk kemenu Fill Black Form, dan isikan data sesuai keinginan, dan kembali kemenu utama.
   6. Kirim hasil form dengan menggunakan menu Send Finalize Form.