# TUGAS_6
- RINO ELJON ATIBAMAN
- 312010006
- TI.20.D.1
- BASIS DATA

- Masuk ke databse nama_nim

![2022-06-01](https://user-images.githubusercontent.com/101688124/171462504-a1690382-1c9a-4890-a094-dd0ec8243cc3.png)

![2022-06-01 (1)](https://user-images.githubusercontent.com/101688124/171462588-8c81fbfc-7844-4e41-8c68-a9a3f62dadd5.png)


- Lakukan proses backup dan recovery dengan sql dari database tugas seblumnya !

Backup

![2022-06-01 (3)](https://user-images.githubusercontent.com/101688124/171463238-c4e0fe25-dbcb-4c2a-a4ea-76c0eb4ca85b.png)


Jika proses backup berhasil maka akan muncul file backuppada direktori C:\xampp\mysql\data\nama database

![2022-06-01 (4)](https://user-images.githubusercontent.com/101688124/171463480-ae883a6e-8e84-47f9-af60-97de49c11daf.png)

Recovery

Data yang telah di-backup dapat dikembalikan kapan saja bila diperlukan. Sintaks SQL yang digunakan adalah LOAD DATA INFILE. Perintah yang dijalankan adalah 

LOAD DATA INFILE ‘Nama_backup_file’ INTO TABLE nama_table ; 


![2022-06-01 (5)](https://user-images.githubusercontent.com/101688124/171464160-1f5dda74-553d-4f4c-94a0-f81c839ae4b1.png)

![2022-06-01 (6)](https://user-images.githubusercontent.com/101688124/171464231-32286e9b-ddee-4c66-ad3d-8eb6891000a6.png)


-  Lakukan proses backup dan recovery dengan sqldump dari database tugas seblumnya !

![2022-06-01 (7)](https://user-images.githubusercontent.com/101688124/171464309-790fe2c1-b8a0-46c4-be4d-38dbf1a9b2a6.png)

![2022-06-01 (8)](https://user-images.githubusercontent.com/101688124/171464340-dcb8eeec-6c10-47c6-b868-e31778fda195.png)



- Tulisakan script cron job untuk melakukan backup otomatis setiap hari minggu jam 12 malam !

crontab –e

00**7myqldump -u root -p rino_312010006>rino_312010006backup.sql
