# Exampp4

#### Nama  : Muhamad Abdul Anas
#### Kelas : TI.22.A2
#### Nim   : 312210269

1# tabel pegawai

#### pertama tama kita buat dulu tabelnya seperti ini
#### Key column 'id_pegawai' doesn't exist in table
#### MariaDB [latihan4]> CREATE TABLE pegawaiper (
####    ->   id_pegawai int(20) NOT NULL AUTO_INCREMENT,
####    ->   nama_depan varchar(25) NOT NULL,
####    ->   nama_belakang varchar(25) NOT NULL,
####    ->   email varchar(25) NOT NULL,
####    ->   telpon int(20) NOT NULL,
####    ->   tgl_kontrak int(20) NOT NULL,
####    ->   id_job int(20) NOT NULL,
####    ->   gaji int(20) NOT NULL,
####    ->   tunjangan int(20) NOT NULL,
####    ->   PRIMARY KEY (id_pegawai)
####    -> );
    
####    lalu lanjut 'desc pegawaiper;'

![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/2fe9102f-07e1-405e-8260-e4e196654b67)

#### selanjutnya kita ketik
#### INSERT INTO pegawaiper (nama_depan, nama_belakang, email, telpon, tgl_kontrak, id_job, gaji, tunjangan)
####    -> VALUES
####    ->   ('ferry', 'gustiawan', 'ferry@yahoo.com', 07117059004, '2005-09-01', 'L0001', 2000000, 500000),
####    ->   ('aris', 'ganiardi', 'aris@yahoo.com', 081312345678, '2006-09-01', 'L0002', 2000000, 200000),
####    ->   ('faiz', 'ahnad', 'faiz@gmail.com', 081367384322, '2006-10-01', 'L0003', 1500000, NULL),
####    ->   ('emna', 'bunton', 'enna@gmail.com', 081363484342, '2006-10-01', 'L0004', 1500000, 9),
####    ->   ('mike', 'scoff', 'mike@plasa.com', 08163454555, '2007-09-01', 'L0005', 1250000, 9),
####    ->   ('licoln', 'burrows', 'linc@yahoo.com', 08527388432, '2008-09-01', 'L0006', 1750000, NULL);
    
    lanjut enter dan 'select *from pegawaiper;'
    ![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/8ac7d665-8916-4896-adec-22a8b90c9ae5)

#### lanjut ke tugas pratikum

#### 1.Tampilkan pegawai yang gajinya bukan 2.000.000 dan 1.250.000 !
#### 'SELECT * FROM pegawaiper WHERE gaji NOT IN (2000000, 1250000);'
 
 ![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/083e8ae3-fdcd-4840-8ab8-e96ddb2ebfd6)
 
#### 2. tampilkan pegawai yang tunjangannya NULL!
#### 'SELECT * FROM pegawaiper WHERE tunjangan IS NULL;'
 
 ![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/a0d6118a-384b-405b-966e-31a585e42029)
 
#### 3. Tampilkan pegawai yang tunjangannya tidak NULL!
#### 'SELECT * FROM pegawaiper WHERE tunjangan IS NOT NULL;'
 
 ![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/199f9327-4d30-48d7-98d0-24db10f704f0)
 
#### 4. Tampilkan/hitung jumlah baris/record tabel pegawai!
#### 'SELECT COUNT(*) FROM pegawaiper;'
 
 ![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/f139742c-3a25-419a-89f2-e5bdccb13090)

#### 5.Tampilkan/hitung jumlah total gaji di tabel pegawai!
#### 'SELECT SUM(gaji) FROM pegawaiper;'

![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/fd773c86-5034-4343-a640-679436e96adf)

### 6.Tampilkan/hitung rata-rata gaji pegawai!
#### 'SELECT AVG(gaji) FROM pegawaiper;'

![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/733e371b-7fc2-492f-9a4c-9dda7711a57f)


#### 7.Tampilkan gaji terkecil!
#### 'SELECT MIN(gaji) FROM pegawaiper;'

![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/d260e170-f62a-4489-9919-873d32b72fc8)


#### 8.Tampilkan gaji terbesar!
#### 'SELECT MAX(gaji) FROM pegawaiper;'

![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/cf6f5150-0d26-45ea-9ed4-44440b80ec88)

2#tabel hewan

#### pertama kita buat dulu tabelnya dengan cara

#### CREATE TABLE hewan2 (
####  id varchar(15) NOT NULL,
####  name varchar(15) NOT NULL,
####  owner varchar(15) NOT NULL,
####  species varchar(15) NOT NULL,
####  sex enum('m', 'f', 'NULL') NOT NULL,
####  PRIMARY KEY (id)
#### lalu enter dan ketik 'desc hewan2;'

![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/7744dfa7-c202-4dec-b391-04d7b50a97cd)

#### selanjutnya ketik
#### INSERT INTO hewan2 (id, name, owner, species, sex)
####    -> values
####    -> ('p1', 'Puffball', 'Diane', 'Hamster', 'f'),
####    ->   ('p2', 'Claws', 'Gwen', 'Cat', 'm'),
####    ->   ('p3', 'Fluffy', 'Haro 1d', 'Cat', 'f'),
####    ->   ('p4', 'Buffy', 'Haro 1d', 'Dog', 'f'),
####    ->   ('p5', 'Fang', 'Benny', 'Dog', 'm'),
####    ->   ('p6', 'Bowser', 'Diane', 'Dog', 'm'),
####    ->   ('p7', 'Chirpy', 'Gwen', 'Bird', 'f'),
####    ->   ('p8', 'Whistler', 'Gwen', 'Bird', NULL),
####    ->   ('p9', 'Slim', 'Benny', 'Snake', 'm');
    
####    lanjut enter dan 'select *from hewan2;'
    ![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/c2ec24df-d631-4f74-acc8-49d8b38c9031)
#### lanjut ke praktikum

####1.Tampilkan jumlah hewan yang dimiliki setiap owner.
#### 'SELECT owner, COUNT(*) as jumlah_hewan FROM hewan2 GROUP BY owner;

![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/70834432-05b1-4c7c-a6e4-f6de6ad26889)

#### 2.Tampilkan jumlah hewan berdasarkan spesies.
'SELECT species, COUNT(*) as jumlah_hewan FROM hewan2 GROUP BY species;'
![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/5cdde6ba-420c-483c-aa5e-f497c0c41471)

#### 3.Tampilkan jumlah hewan berdasarkan jenis kelamin.
'SELECT sex, COUNT(*) as jumlah_hewan FROM hewan2 GROUP BY sex;'
![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/28b77abf-2a85-4e09-adb8-58080184e02a)


#### 4.Tampilkan jumlah hewan berdasarkan spesies dan jenis kelamin.
'#### SELECT species, sex, COUNT(*) as jumlah_hewan FROM hewan2 GROUP BY species, sex;'
![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/3146659e-7f84-4de8-b052-a2a77a1bbf2f)


#### 5.Tampilkan jumlah hewan berdasarkan spesis (cat dan dog saja) dan jenis kelamin.
#### SELECT species, sex, COUNT(*) as jumlah_hewan
####    -> FROM hewan2
 ####   -> WHERE species IN ('Cat', 'Dog')
 ####   -> GROUP BY species, sex;
![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/7c787489-1f1e-4e73-99ea-18259bcb1df1)


#### 6.Tampilkan jumlah hewan berdasarkan jenis kelamin yang diketahui saja.
#### SELECT sex, COUNT(*) as jumlah_hewan
####    -> FROM hewan2
####    -> WHERE sex IS NOT NULL
####    -> GROUP BY sex;
![image](https://github.com/muhamadabdulanas/prakexamp5/assets/115569493/83cc5be3-03e0-4b47-bee7-a54610cbb933)


#### #Evaluasi dan Pertanyaan

#### kesimpulan

#### Dari percobaan SQL yang saya lakukan, dapat disimpulkan yaitu tabel "pegawaiper" telah berhasil dibuat dan diisi dengan data pegawai. quary-quary yang dilakukan berhasil menghasilkan output yang sesuai dengan kondisi yang di tentukan. Data dalam tabel dapat digunakan untuk analisis lebih lanjut seperti menghitung jumlah pegawai, total gaji, rata-rata gaji, gaji terkecil, dan gaji terbesar.





