# pert.12
<p>buat program sederhana dengan mengaplikasikan penggunaan class.
Buatlah class untuk menampilkan ddaftar nilai mahasiswa,dengan ketentuan:</p>
<p>• Method tambah() untuk menambah data</p>
<p>• Method tampilkan() untuk menampilkan data</p>
<p>• Method hapus(nama) untuk menghapus data berdasarkan nama</p>
<p>• Method ubah(nama) untuk mengubah data berdasarkan nama</p>
<p>• Buat diagram class, flowchart dan penjelasan programnya pada
README.md.</p>
<p>• Commit dan push repository ke github.</p>

# <p>masukkan kode program</p>

def hapus(nama):
    print(f"{'Data Berhasil di Hapus':^17}")
    print('='*17)
    del data[nama]

def ubah(nama):
    print(f"{'Ubah Data':^17}")
    print('='*17)
    nim = str(input('NIM\t\t: ')) 
    uts = int(input('Nilai UTS\t: '))
    uas = int(input('Nilai UAS\t: '))
    tugas = int(input('Nilai Tugas\t: '))
    akhir = round(float((tugas*0.3)+(uts*0.35)+(uas*0.35)),2)
    data[nama] = nim, uts, uas, tugas, akhir

def salah():
    print(f"{'Daftar Data Mahasiswa':^82}")
    print('='*84)
    print(f"|{'NO':^4}|{'NIM':^20}|{'NAMA':^20}|{'TUGAS':^10}|{'UTS':^6}|{'UAS':^6}|{'AKHIR':^10}|")
    print('='*84)
    print(F"|{'Tidak ada data':^82}|")
    print('='*84)
    
# <p>menambahkan data</p>

![prakt 8](https://github.com/endangsirait/pert.12/assets/148036197/e0e17ec7-7156-4963-8b39-53d480c79420)
![prakt8](https://github.com/endangsirait/pert.12/assets/148036197/00500416-e0ba-40f3-b30d-aebff3b6cd5a)

# <p> menampilkan data</p>

![praktik8](https://github.com/endangsirait/pert.12/assets/148036197/c5f830c8-2d41-49d0-89af-f9f64c64fecf)

# <p> menghapus data</p>

![praktik8 (2)](https://github.com/endangsirait/pert.12/assets/148036197/51223638-4819-48a3-915b-ace449b30355)

# <p> mengubah data</p>

![praktik8 (3)](https://github.com/endangsirait/pert.12/assets/148036197/e6bcd3e9-0702-4ce4-b565-5373108b5feb)

# <p> keluar aplikasi</p>

![praktik8 (4)](https://github.com/endangsirait/pert.12/assets/148036197/88d67a8e-f4f0-4c55-8d56-64fe4d9dfead)

# <p> Diagram class</p>

<img width="415" alt="diagramclass" src="https://github.com/endangsirait/pert.12/assets/148036197/a10ce3aa-0e54-47c6-bd67-560f83871e26">

# <p> flowchart</p>

<img width="425" alt="Flowchart (1)" src="https://github.com/endangsirait/pert.12/assets/148036197/4b1109f3-735e-4d28-b35e-8d490dbc41c5">

