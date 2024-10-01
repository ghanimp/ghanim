# ghanim
Nama : Ghani Mandala Putra, Nim 2409116042, Proyek 1

![mini project  drawio (1)](https://github.com/user-attachments/assets/bc49676b-2bab-4e77-8981-a937173e151b)

![Screenshot 2024-10-01 101048](https://github.com/user-attachments/assets/68e5d124-adc2-4d48-9f4d-5875624bbd84)

1.saya membuat proses login sederhana 

2.disini menggunakan while true agar bisa melakukan login ulang 

3.kemudian ada input untuk memasukkan nama dan nim


![Screenshot 2024-10-01 102141](https://github.com/user-attachments/assets/9c4be7a0-d7c2-4633-b61b-d9bd7d30b370)

4.disini saya isi nama dan nim  sesuai dengan nama saya

5.saya menambahkan opsi login ulang atau tidak

6.menambahkan break untuk menghentikan program mengulang lagi dan untuk lanjut ke bagian selanjutnya

![Screenshot 2024-10-01 102936](https://github.com/user-attachments/assets/0c7323ea-cb0e-4dc5-aa1f-7d7eb9e85dea)

7.jika nama dan nim salah ada opsi untuk mengulang memasukkan nama dan nim

8.jika memilih tidak mengulang program akan berakhir

![Screenshot 2024-10-01 103922](https://github.com/user-attachments/assets/6d922bdb-2436-4e33-9d16-b737f1877c22)

9.saya kembali menggunakan while true agar bisa mengulang program

10.di sini saya memberikan rumus untuk menghitung total jumlah pembelian

![Screenshot 2024-10-01 104050](https://github.com/user-attachments/assets/5230daef-c463-4048-b881-0d4143367fa5)

11.selanjutnya saya memberikan perintah jika jumlah total harga > 250000, maka akan mendapatkan diskon

12.dan saya berikan rumus lagi untuk menghitung harga akhir

![Screenshot 2024-10-01 104530](https://github.com/user-attachments/assets/53e6a22a-8fed-4008-ac55-b486913d6ee9)

13.selanjutnya saya memberikan pilihan lagi untuk mengulang atau tidak

14.jika memilih ulang maka akan kembali menginput harga barang, namun jika memilih tidak program akan selesai

![Screenshot 2024-10-01 104812](https://github.com/user-attachments/assets/07eddf47-47f6-432b-8924-083d9e987f39)

15.namun jika jumlah total harga barang < 250000, maka tidak akan mendapatkan diskon

16.saya juga menambahkan opsi untuk mengulang atau mengakhiri program

BERIKUT HASILNYA

#Ghani Mandala Putra
#2409116042
#SI 24 B

#login sederhana
while True:
    print("__________Login___________")
    print("Masukkan Nama dan NIM anda")
    nama = str(input("Masukkan Nama anda: "))
    nim = str(input("Masukkan NIM anda: "))
    if nama == "Ghani" and nim == "2409116042":
        print("Selamat datang,",nama,"Dengan NIM",nim)
        ulang = input("Apakah Anda ingin mencoba login lagi? (y/n): ")
        if ulang != 'y': break 
    else:
        print("Nama atau NIM anda tidak dikenal")
        ulang = input("Apakah Anda ingin mencoba login lagi? (y/n): ")
        if ulang != 'y':
            print("Login Gagal")
            exit()

#mennghitung total harga
while True:
    #mengisi jumlah dan harga barang
    harga_barang = int(input("Masukkan harga barang: Rp. "))
    jumlah_barang = int(input("Masukkan jumlah barang: "))
    total_harga = harga_barang * jumlah_barang

    #proses menentukan akan mendapatkan diskon atau tidak
    if total_harga > 250000:
        harga_akhir = total_harga - (0.25 * total_harga)
        print("Selamat, Anda Mendapatkan Diskon 25%")
        print("Total harga adalah: Rp. ",harga_akhir)
        ulang = input("Apakah anda ingin menghitung barang lagi? (y/n): ")
        if ulang == 'y':  #pengulangan jika ingin mengulang
            lanjut = 'y'
        
        else:
            print("Program Selesai")
            exit()

    else:
        print("Total harga adalah: Rp. ",total_harga)
        ulang = input("Apakah anda ingin menghitung barang lagi? (y/n): ")
        if ulang == 'y':
            lanjut = 'y'
        
        else:
            print("Program Selesai")
            exit()


![Screenshot 2024-10-01 094449](https://github.com/user-attachments/assets/ca99e296-a85e-408e-b25c-946d7b04e2e8)

Ini adalah percobaan yang saya lakukan saat menjalankan programnya


