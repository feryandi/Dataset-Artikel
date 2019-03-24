# Dataset: Artikel
Proyek ini awalnya dilakukan untuk mempelajari infrastruktur Google Cloud Platform, sehingga masih banyak kekurangan dari segi data. Selain itu, terinspirasi juga dari proyek https://github.com/ParallelMazen/SaudiNewsNet yang mengumpulkan data serupa.

Proyek inisiatif untuk membuka akses kepada publik terhadap ribuan artikel berbahasa Indonesia dari berbagai sumber beserta metadata artikel tersebut. **Artikel yang ada disini masih mentah (raw) dan tidak berlabel.**
Diharapkan akan mempermudah akses mendapatkan set mentah data artikel dari berbagai sumber untuk keperluan pembelajaran, penelitian, dan pengembangan kakas pemrosesan Bahasa Indonesia.

## Akses data
Data dapat diakses pada Google Drive yang dapat diakses, diunduh, dan digunakan oleh publik. Dengan mengakses tautan tersebut, Anda telah setuju dengan Ketentuan Penggunaan Data.

[<img src="https://www.google.com/drive/static/images/drive/logo-drive.png" width="20"> Menuju Google Drive](https://drive.google.com/drive/folders/12KdmXUxssdL5nKYz5afolHqHEW_fdCFI?usp=sharing)

## Konten
### Tipe Berkas
Pada Google Drive tersebut, terdapat dua folder yang bernamakan `json` dan `html`. Pada folder `json`, terdapat berkas-berkas yang berisikan artikel-artikel yang sudah melalui proses pembersihan sehingga hanya berisi konten. Pada folder `html`, terdapat berkas-berkas mentah berupa file html yang diambil langsung dari sumbernya.

### Struktur Folder
Struktur folder akan mengikuti tanggal artikel tersebut dikeluarkan. Sturkturnya secara umum adalah sebagai berikut,
`{tipe}/{tahun}/{tanggal}/{hari}/{jam}/{timestamp}.{nama-media}.{hash-judul}.{tipe}`

Contohnya `json/2018/05/02/02/1525226400000.cnn-indonesia.fe5490cb31.json` merujuk pada artikel CNN Indonesia yang ditayangkan pada tanggal 02 Mei 2018 pada pukul 2 pagi.

### Statistik
##### Jumlah Artikel
Artikel diambil dari untuk rentang waktu 01 Januari 2018 hingga 20 Agustus 2018 untuk media-media berikut:
<table>
<colgroup>
  <col style="text-align:left;"/>
  <col style="text-align:left;"/>
</colgroup>

<thead>

<tr>
    <th style="text-align:left;">Media</th>
    <th style="text-align:left;">#</th>
</tr>
</thead>

<tbody>
<tr>
    <td style="text-align:left;">Detik</td>
    <td style="text-align:left;">85,802</td>
</tr>
<tr>
    <td style="text-align:left;">Kompas</td>
    <td style="text-align:left;">60,902</td>
</tr>
<tr>
    <td style="text-align:left;">Tempo</td>
    <td style="text-align:left;">44,409</td>
</tr>
<tr>
    <td style="text-align:left;">CNN Indonesia</td>
    <td style="text-align:left;">24,965</td>
</tr>
<tr>
    <td style="text-align:left;">Sindo</td>
    <td style="text-align:left;">34,002</td>
</tr>
<tr>
    <td style="text-align:left;">Republika</td>
    <td style="text-align:left;">64,008</td>
</tr>
<tr>
    <td style="text-align:left;">Poskota</td>
    <td style="text-align:left;">17,747</td>
</tr>
<tr>
    <td style="text-align:left;">Lainnya</td>
    <td style="text-align:left;">2</td>
</tr>
</tbody>
</table>


##### Statistik Dataset
Dataset berisikan 109.192.608 token (dihitung menggunakan tokenizer NLTK, lowercase, angka dianggap unik, serta belum dibersihkan) dan 659.066 token unik.
Peringkat 22 kata dengan kemunculan terbanyak adalah sebagai berikut,
![Statistik Kata](/img/statistik_kata.png?raw=true)

![Grafik Kemunculan Kata](/img/kemunculan_kata.png?raw=true "Grafik Kemunculan Kata")

## Kontak Pengelola
Jika Anda ingin menghubungi pengelola data ini silakan kontak menggunakan media berikut ini,
- **Email :** feryandi [dot] n [at] gmail [dot] com

## Ketentuan Penggunaan Data
* Tidak ada batasan pada penggunaan, namun mohon gunakan secara bertanggungjawab.
* Ikuti lisensi atau izin yang berlaku terhadap data ini (lihat: Izin Penggunaan)
* Tidak ada pungutan biaya apapun dalam penggunaan, namun untuk mengelola data ini tetap diperlukan biaya. Jika Anda merasa terbantu, mohon lakukan donasi untuk proyek ini.

## Izin Penggunaan
![Creative Commons Attribution-ShareAlike 4.0 International License](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)

##### [ Indonesia ]
Proyek ini dilisensikan dibawah lisensi **Creative Commons Attribution-ShareAlike 4.0 International License**. Kumpulan data yang dibagikan bertujuan untuk ilmu pengetahuan, pembelajaran, dan penelitian Bahasa Indonesia (komputasi maupun lingusitik), dan hanya dapat digunakan untuk hal tersebut. Kepemilikan data untuk setiap artikel dimiliki oleh media dan surat kabar yang bersangkutan dimana data tersebut diambil; dan pemilik _repository_ ini tidak melakukan klaim kepemilikan atas konten tersebut. Jika Anda mendapati bahwa data ini telah melanggar suatu hak cipta; mohon kontak pengelola _repository_ ini. 

##### [ English ]
This work is licensed under a **Creative Commons Attribution-ShareAlike 4.0 International License**. The dataset is shared for the sole purpose of aiding open scientific research in Bahasa Indonesia (computing or linguistics), and can only be used for that purpose. The ownership of each article within the dataset belongs to the respective newspaper from which it was extracted; and the maintainer of the repository does not claim ownership of any of the content within it. If you think, by any means, that this dataset breaches any established copyrights; please contact the repository maintainer.

