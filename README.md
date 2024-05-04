# Experiment README
## Experiment 2.1: Original code, and how it run
![alt text](runserver.png)  
![alt text](client1.png)  
![alt text](client2.png)  
![alt text](client3.png)  
- Dari output di atas dapat kita lihat bahwa server akan menjadi listener dan menerima connection dari tiap client. Dapat kita lihat Server akan menerima dan memberikan message baru yang diberikan. Setiap client dapat membuat message dan menerima message dari client lain yang terkoneksi dan diproses oleh server.

## Experiment 2.2: Modifying port
![alt text](runserver2.png)  
![alt text](client1.2.png)  
![alt text](client2.2.png)  
![alt text](client3.2.png)  
- Apabila kita mengganti port server dan client dengan port yang sama. Maka, aplikai akan tetap berjalan dengan baik seperti gambar di atas.
![alt text](error.png)  
- Namun, jika kita mengganti salah 1 port client atau server maka akan muncul error karena client tidak menemukan target server dengan port yang sesuai seperti foto di atas.
