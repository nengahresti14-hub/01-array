# penjelasan array
nilai_mahasiswa=[] digunakan untuk medefinisikan sebuah array,data nilai mahasiswa di simpan di list kosong[]


![alt text](https://github.com/nengahresti14-hub/01-array/blob/main/Foto/Screenshot_2026-03-14-10-26-04-578_com.android.chrome-edit.jpg?raw=true)

![alt text](https://github.com/nengahresti14-hub/01-array/blob/main/Foto/Screenshot_2026-03-14-10-26-23-711_com.android.chrome-edit.jpg?raw=true)
(for i in range(10):):
Baris ini melakukan pekerjaan yang sama atau looping sebanyak 10 putaran. Program akan menghitung mulai dari putaran ke-0 hingga ke-9.

append(n): Inilah bagian paling penting. Fungsi ini akan mengambil angka yang baru saja dimasukkan dan memasukkannya ke dalam Array nilai_mahasiswa.
## mencari nilai tertinggi dan terendah
![alt text](https://github.com/nengahresti14-hub/01-array/blob/main/Foto/Screenshot_2026-03-14-11-00-13-605_com.android.chrome-edit.jpg?raw=true)
#### nilai_tertinggi = max(nilai_mahasiswa)
Baris ini mencari angka paling besar di dalam daftar (array) nilai_mahasiswa dan menyimpannya ke variabel nilai_tertinggi.
#### nilai_terendah = min(nilai_mahasiswa)
Baris ini mencari angka paling kecil di dalam daftar tersebut dan menyimpannya ke variabel nilai_terendah.
#### print(f"Nilai tertinggi{nilai_tertinggi}")
Menampilkan teks ke layar yang berisi hasil nilai paling besar yang sudah ditemukan tadi.

#### print(f"Nilai terendah{nilai_terendah}")
Menampilkan teks ke layar yang berisi hasil nilai paling kecil yang sudah ditemukan tadi.

## Mencari Rata Rata Nilai
![alt text](https://github.com/nengahresti14-hub/01-array/blob/main/Foto/Screenshot_2026-03-14-11-00-33-333_com.android.chrome-edit.jpg?raw=true)
#### rata_rata = sum(nilai_mahasiswa) / len(nilai_mahasiswa)
Baris ini menjumlahkan seluruh angka di dalam daftar (sum) lalu membaginya dengan total jumlah data yang ada (len atau length) untuk mendapatkan nilai tengah.
#### print(f"Rata-rata nilai: {rata_rata}")
Menampilkan hasil perhitungan pembagian tersebut ke layar dengan format teks.

## Menghitung jumlah mahasiswa lulus dengan ketentuan nilai di atas atau sama dengan 60 lulus
![alt text](https://github.com/nengahresti14-hub/01-array/blob/main/Foto/Screenshot_2026-03-14-11-00-47-624_com.android.chrome-edit.jpg?raw=true)
#### ​jumlah_lulus = 0
Menyiapkan sebuah variabel penghitung (counter) yang dimulai dari angka nol untuk mencatat berapa banyak mahasiswa yang lulus.
#### ​for nilai in nilai_mahasiswa:
Melakukan pengecekan satu per satu terhadap setiap angka yang ada di dalam daftar (list) nilai.
#### ​if nilai >= 60:
Sebuah syarat (kondisi) di mana hanya nilai yang sama dengan atau lebih besar dari 60 yang akan diproses lebih lanjut.
#### ​jumlah_lulus += 1
Jika nilai memenuhi syarat (60 ke atas), maka angka pada penghitung akan bertambah 1.
#### ​print(f"Jumlah mahasiswa yang lulus: {jumlah_lulus}")
Menampilkan hasil akhir jumlah total mahasiswa yang berhasil melewati ambang batas nilai tersebut.

## Membuat grafik untuk menggambarkan nilai tertinggi dan terendah
![alt text](https://github.com/nengahresti14-hub/01-array/blob/main/Foto/Screenshot_2026-03-14-14-07-04-519_com.android.chrome-edit.jpg?raw=true)

#### import matplotlib.pyplot as plt
Memanggil library (perpustakaan kode) Matplotlib yang berfungsi untuk menggambar grafik atau diagram.
#### ​nama_nilai = [...] & values = [...]
Menyiapkan label (nama) dan data angka yang akan dimasukkan ke dalam grafik.
#### ​plt.figure(figsize=(7, 5))
Mengatur ukuran jendela atau kanvas grafik yang akan dibuat (lebar 7 inci, tinggi 5 inci).
#### ​plt.bar(..., color=[...])
Perintah utama untuk membuat diagram batang dengan warna biru langit dan merah muda.
#### ​plt.title, plt.ylabel, plt.ylim
Memberikan judul grafik, label pada garis tegak (Y), dan membatasi rentang angka dari 0 sampai 100.
#### ​for i, val in enumerate(values):
Sebuah perulangan untuk menuliskan angka nilai tepat di atas setiap batang grafik agar lebih mudah dibaca.
#### ​plt.show()
Perintah terakhir untuk memunculkan jendela grafik ke layar.

## Membuat grafik untuk menggambarkan data kelulusan
![alt text](https://github.com/nengahresti14-hub/01-array/blob/main/Foto/Screenshot_2026-03-14-14-07-24-575_com.android.chrome-edit.jpg?raw=true)
#### Menghitung Total Mahasiswa
​total_mahasiswa = len(nilai_mahasiswa): Menghitung jumlah total seluruh mahasiswa yang ada di dalam daftar (list).
#### ​Menghitung Mahasiswa Tidak Lulus
​jumlah_tidak_lulus = total_mahasiswa - jumlah_lulus: Mencari selisih untuk mengetahui berapa banyak mahasiswa yang tidak mencapai nilai ambang batas.
#### ​Menyiapkan Data Grafik
​labels = [...] & sizes = [...]: Menentukan teks keterangan ("Lulus/Tidak Lulus") dan data angka yang akan ditampilkan pada grafik.
#### ​Membuat Grafik Batang
​plt.bar(labels, sizes, color=colors): Membuat grafik batang dengan warna hijau untuk yang lulus dan merah untuk yang tidak lulus.
#### ​Mengatur Batas Sumbu Y
​plt.ylim(0, total_mahasiswa + 2): Mengatur batas tinggi grafik agar sedikit lebih tinggi dari jumlah total mahasiswa supaya tampilan tidak terpotong.
#### ​Menampilkan Label Angka
​plt.text(...): Menaruh angka jumlah mahasiswa tepat di atas masing-masing batang grafik sebagai label data.
#### ​Menampilkan Visualisasi
​plt.show(): Menampilkan hasil akhir visualisasi grafik perbandingan kelulusan tersebut ke layar.
# HASIL SCREENSHOT
![alt text](https://github.com/nengahresti14-hub/01-array/blob/main/Foto/Screenshot_2026-03-14-16-56-25-719_com.android.chrome-edit.jpg?raw=true)
![alt text](https://github.com/nengahresti14-hub/01-array/blob/main/Foto/Screenshot_2026-03-14-16-56-40-333_com.android.chrome-edit.jpg?raw=true)
![alt text](https://github.com/nengahresti14-hub/01-array/blob/main/Foto/Screenshot_2026-03-14-16-57-00-978_com.android.chrome-edit.jpg?raw=true)
![alt text](https://github.com/nengahresti14-hub/01-array/blob/main/Foto/Screenshot_2026-03-14-16-58-09-532_com.android.chrome-edit.jpg?raw=true)
![alt text](https://github.com/nengahresti14-hub/01-array/blob/main/Foto/Screenshot_2026-03-14-16-58-51-326_com.android.chrome-edit.jpg?raw=true)
![alt text](https://github.com/nengahresti14-hub/01-array/blob/main/Foto/Screenshot_2026-03-14-16-59-10-178_com.android.chrome-edit.jpg?raw=true)

