# praktikum-8

# NAMA : GALVA AL GODZALI

# NIM : 312210356

# KELAS : TI.22.A.3

Tugas membuat program sederhana

![praktikum 8 tugas](https://user-images.githubusercontent.com/115516730/206966574-2b224057-9642-4c21-a0f4-08ea52d7ccb9.png)

Kode dari tugas tersebut ialah 
print('====program menambah data dengan class=====')
mahasiswa = {}

class daftarNilai():

    def tambah(self):
        print('\nTambah Data Mahasiswa')
        nama = input("Masukkan Nama\t\t: ")
        nim = input("Masukkan NIM\t\t: ")
        nilaiTugas = int(input("Masukkan Nilai Tugas\t: "))
        nilaiUts = int(input("Masukkan Nilai UTS\t: "))
        nilaiUas = int(input("Masukkan Nilai UAS\t: "))
        nilaiAkhir = (0.30 * nilaiTugas) + (0.35 * nilaiUts) + (0.35 * nilaiUas)
        mahasiswa[nama] = nim, nilaiTugas, nilaiUts, nilaiUas, nilaiAkhir,
        print("\nData Berhasil Di Ditambahkan!\n")

    def ubah(self):
        print('\nMengubah Data Mahasiswa')
        nama = input("Masukkan Nama: ")
        if nama in mahasiswa.keys():
            nim = input("Masukkan NIM Baru\t: ")
            nilaiTugas = int(input("Masukkan Nilai Tugas\t: "))
            nilaiUts = int(input("Masukkan Nilai UTS\t: "))
            nilaiUas = int(input("Masukkan Nilai UAS\t: "))
            nilaiAkhir = (30/100 * nilaiTugas) + (35/100 * nilaiUts) + (35/100 * nilaiUas)
            mahasiswa[nama] = nim, nilaiTugas, nilaiUts, nilaiUas, nilaiAkhir
            print("\nData Berhasil Di Update!\n")
        else:
            print("Data tidak ditemukan!\n")

    def hapus(self):
        print('\nmenghapus data')
        nama = input("Masukkan Nama:  ")
        if nama in mahasiswa.keys():
            del mahasiswa[nama]
            print("\nData Telah dihapus!\n")
        else:
            print("Data Mahasiswa Tidak Ada\n")

    def lihat(self):
        if mahasiswa.items():
            print("\n                      DAFTAR NILAI MAHASISWA                    ")
            print("==================================================================")
            print("| No |     Nama     |    NIM    | Tugas |  UTS  |  UAS  |  Akhir |")
            print("==================================================================")
            i = 0
            for x in mahasiswa.items():
                i += 1
                print("| {6:2} | {0:12s} | {1:9s} | {2:5} | {3:5} | {4:5} | {5:6} |".format(x[0], x[1][0], x[1][1],
                                                                                            x[1][2], x[1][3], x[1][4],
                                                                                            i))
            print("==================================================================\n")
        else:
            print("\n                      DAFTAR NILAI MAHASISWA                    ")
            print("==================================================================")
            print("| No |     Nama     |    NIM    | Tugas |  UTS  |  UAS  |  Akhir |")
            print("==================================================================")
            print("|                          TIDAK ADA DATA!                       |")
            print("==================================================================\n")

    def keluar(self):
        print('\n=====terimakasih=====\n')
        print(21 * '=')
        print("Nama\t: Rini Ariza\nKelas\t: TI.22.A3\nNIM\t: 312210337")
        print(21 * '=')


while True : 

    data = daftarNilai()
    
    print('\ntambah\t(1)\nubah\t(2)\nlihat\t(3)\nhapus\t(4)\nkeluar\t(5)')
    
    c = input("\nsilahkan masukan pilihan : ")
    
    print()
    if (c == "1"):
        data.tambah()
    elif (c == "2"):
        data.ubah()
    elif (c == "3"):
        data.lihat()
    elif (c == "4"):
        data.hapus()
    elif (c == "5"):
        data.keluar()
        break

    else:
        print()
        print("Kode yang anda masukkan salah!")
        
 Maka OUTPUT yand didapatkan berupa bebrapa pilihan seperti yang tertera pada gambar berikut ini
 
 ![p1](https://user-images.githubusercontent.com/115516730/206967075-6c7f963d-f33a-4168-8118-39e634fb516c.png)
 
 Tidak lupa saya memberikan flowchar program seperti berikut ini:
 
 <img width="543" alt="p2" src="https://user-images.githubusercontent.com/115516730/206967258-046d6c14-8bcc-473e-8779-bd7833c2b17c.png">
 
 Sekian dari yang saya dapat sampaikan kurang lebihnya mohon dimaafkan terima kasih

