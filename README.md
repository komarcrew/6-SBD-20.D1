# PRAKTIKUM SISTEM BASIS DATA
Nama  : Komarudin <p>
NIM   : 312010068 <p>
Kelas : TI.20.D.1 <p>
## Tugas 6 : Backup dan Restore pada MySQL <p>
### 1.Masuk ke database nama_nim<p>
![image](https://user-images.githubusercontent.com/101499377/171459185-3f7790c3-c0de-49d8-a2fd-6d326d4a9e30.png)<p>
### 2.Lakukan proses backup dan recovery dengan sql dari database tugas seblumnya !<p>
Proses Backup.<p>
  ![image](https://user-images.githubusercontent.com/101499377/171459762-0882265b-bd86-4692-b1e4-b3ef04a0e283.png)<p>
Jika proses backup berhasil maka akan muncul file pada direktori C:\xampp\mysql\data\nama database<p>
![image](https://user-images.githubusercontent.com/101499377/171460273-e3cf8e31-e303-458f-9e2a-2bb4f6c6d196.png)<p>
Proses Recovery.<p>
Data yang telah di-backup dapat dikembalikan kapan saja dan Syntax yang digunakan di MySQL adalah LOAD DATA INFILE ‘Nama_backup_file’ INTO TABLE nama_table ;<p>
![image](https://user-images.githubusercontent.com/101499377/171464127-6d68175e-d9c4-4f88-a5a2-2b640ef026d0.png)<p>
### 3.Lakukan proses backup dan recovery dengan sqldump dari database tugas seblumnya !<p>
![image](https://user-images.githubusercontent.com/101499377/171465056-0bb35dc0-9591-4736-8043-97a2454a4e1f.png)<p>
### 4.Tulisakan script cron job untuk melakukan backup otomatis setiap hari minggu jam 12 malam !<p>
0 0 * * 7 mysqldump -u root –p komarudin_312010068>komarudin_312010068_backup.sql<p>
