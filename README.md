# Experiment README
## Experiment 2.1: Original code, and how it run
![alt text](/public/runserver.png)  
![alt text](/public/client1.png)  
![alt text](/public/client2.png)  
![alt text](/public/client3.png)  
- Dari output di atas dapat kita lihat bahwa server akan menjadi listener dan menerima connection dari tiap client. Dapat kita lihat Server akan menerima dan memberikan message baru yang diberikan. Setiap client dapat membuat message dan menerima message dari client lain yang terkoneksi dan diproses oleh server.

## Experiment 2.2: Modifying port
![alt text](/public/runserver2.png)  
![alt text](/public/client1.2.png)  
![alt text](/public/client2.2.png)  
![alt text](/public/client3.2.png)  
- Apabila kita mengganti port server dan client dengan port yang sama. Maka, aplikai akan tetap berjalan dengan baik seperti gambar di atas.
![alt text](/public/error.png)  
- Namun, jika kita mengganti salah 1 port client atau server maka akan muncul error karena client tidak menemukan target server dengan port yang sesuai seperti gambar di atas.

## Experiment 2.3: Small changes, add IP and Port
![alt text](/public/servermodif.png) 
![alt text](/public/clientmodif.png) 
![alt text](/public/clientmodif2.png) 
- Saya menambahkan informasi from `venedictchen's computer` pada server dan client. Saya menambahkan `bcast_tx.send(format!("{addr} : {text}"))?;` agar memberikan pesan broadcast dengan format address dan textnya sehingga semua client mendapatkan informasi dari tiap address client lain. Lalu, saya juga menambahkan `println!("New connection from venedictchen's computer {addr:?}");` untuk menambahkan informasi connection ke server `venedictchen's computer` terjadi.