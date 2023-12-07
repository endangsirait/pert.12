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
data={} 
import os
class data_mahasiswa():
    def tambah():
        print(f"{'Tambah Data':^17}")
        print('='*17)
        nim = str(input('NIM\t\t: '))
        nama = str(input('Nama\t\t: '))
        uts = int(input('Nilai UTS\t: '))
        uas = int(input('Nilai UAS\t: '))
        tugas = int(input('Nilai Tugas\t: '))
        akhir = round(float((tugas*0.3)+(uts*0.35)+(uas*0.35)),2)
        data[nama]=nim, uts, uas, tugas, akhir
    def tampilkan():
        print(f"{'Daftar Data Mahasiswa':^82}")
        print('='*84)
        print(f"|{'NO':^4}|{'NIM':^20}|{'NAMA':^20}|{'TUGAS':^10}|{'UTS':^6}|{'UAS':^6}|{'AKHIR':^10}|")
        print('='*84)
        n = 0
        for a in data.items():
            n += 1
            print("|{no:^4}|{0:^20}|{1:^20}|{2:^10}|{3:^6}|{4:^6}|{5:^10}|"
            .format(a[1][0], a[0][:13], a[1][1], a[1][2], a[1][3], a[1][4], no = n))
        print('='*84)

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
while True:
    print()
    lanjut = str(input('MENU\n=======\n(L)ihat\n(T)ambah\n(U)bah\n(H)apus\n(K)eluar\n=======\nPilihan : '))
    os.system("cls")
    if lanjut.lower() == 'l':
        if data.items():
            data_mahasiswa.tampilkan()
        else:
            data_mahasiswa.salah()
    elif lanjut.lower() == 't':
            data_mahasiswa.tambah()
    elif lanjut.lower() == 'h':
        print('Data yang ingin di hapus')
        nama = str(input('Nama\t\t: '))
        if nama in data.keys():
            data_mahasiswa.hapus(nama)
        else:
            data_mahasiswa.salah()
    elif lanjut.lower() == 'u':
        print('Data yang ingin di ubah')
        nama = str(input('Nama\t\t: '))
        if nama in data.keys():
            data_mahasiswa.ubah(nama)
        else:
            data_mahasiswa.salah()
    elif lanjut.lower() == 'k':
        break
    else :
        print('Pilih menu yang tersedia')
print('Program Selesai')

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



