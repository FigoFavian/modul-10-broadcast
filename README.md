
## 2.1 Original code and How It Runs

### Server 

Server memiliki kewajiban sebagai _listener_ yang menerima _connection_ dari setiap Client. Server akan menerima tiap pesan dari berbagai Client dan kemudian akan memberitakan pesan yang baru. Client dapat menerima pesan dari Client lainnya yang terkoneksi ke Server.

Bukti:

![alt text](image.png)

### Client 1 

bukti:

![alt text](image-1.png)

### Client 2 

bukti:

![alt text](image-2.png)

### Client 3 

bukti:

![alt text](image-3.png)

### Client 4

bukti:

![alt text](image-4.png)

##  2.2: Modifying the websocket port 

Jika port berbeda (Antar client dan server) maka akan error. Hal ini terjadi karena Client tidak menemukan target Server dengan port yang sesuai.

Bukti:

![alt text](image-5.png)

Namun jika kedua port (di client dan sever) sama, semisal keduanya diubah ke port 8080, maka akan berhasil dan broadcast akan berjalan seperti biasanya.

Bukti:

![alt text](image-6.png)

### Client 1

![alt text](image-7.png)

### Client 2

![alt text](image-8.png)

## 2.3 Small Changes by Adding Some Information to Client

Saya menambah keterangan bahwa koneksi terjadi di Figo's Computer dan juga agar semua Client dapat melihat _address_ Client lain. 

Bukti:

![alt text](image-10.png)

![alt text](image-11.png)

![alt text](image-12.png)

![alt text](image-13.png)