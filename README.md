# MINPRO-DPP
Alya Aulia - Sistem Informasi


NAMA : ALYA AULIA
NIM : 2509116060
PRODI : SISTEM INFORMASI - B


FLOWCHART














KONDISI 1

<img width="891" height="261" alt="Output Kondisi 1" src="https://github.com/user-attachments/assets/dfca3dad-f7e1-4593-a49e-19343ffa2eb8" />

KONDISI 2

<img width="880" height="256" alt="Output Kondisi 2" src="https://github.com/user-attachments/assets/6e369649-ba11-4b8d-8cd9-00e836427e6d" />

KONDISI 3

<img width="858" height="252" alt="Output Kondisi 3" src="https://github.com/user-attachments/assets/1b31c25d-e0d6-4adb-9891-f98f706d6fc6" />

KONDISI 4

<img width="788" height="197" alt="Output Kondisi 4" src="https://github.com/user-attachments/assets/be02e34b-8fee-4834-a8e9-7ade3fd4d88d" />

KONDISI 5

<img width="834" height="169" alt="Output Kondisi 5" src="https://github.com/user-attachments/assets/a678d7bf-6ae7-4f8d-800e-6da704a0eea3" />

KONDISI 6

<img width="898" height="293" alt="Output Kondisi 6" src="https://github.com/user-attachments/assets/ff31db99-94a9-44e9-93a5-19530107ea13" />

KONDISI 7

<img width="913" height="244" alt="Output Kondisi 7" src="https://github.com/user-attachments/assets/8837497b-b5ed-41b9-920c-01848e1bf970" />

KONDISI 8

<img width="913" height="252" alt="Output Kondisi 8" src="https://github.com/user-attachments/assets/1e71e06b-b475-430a-970d-d64a88e42d2c" />

KONDISI 9

<img width="919" height="263" alt="Output kondisi 9" src="https://github.com/user-attachments/assets/c2e37004-a26d-4768-a840-93430574e014" />

KONDISI 10

<img width="981" height="203" alt="Output Kondisi 10" src="https://github.com/user-attachments/assets/189ccb0e-40cd-4b14-80dc-ca3539d7891e" />

KONDISI 11

<img width="867" height="112" alt="Output Kondisi 11" src="https://github.com/user-attachments/assets/8a4472d1-4e7c-401e-b6da-c2ca30c96ce4" />

KONDISI 12

<img width="962" height="131" alt="Output Kondisi 12" src="https://github.com/user-attachments/assets/5b990ee6-adcd-479a-af8a-cdcd73a90f66" />

KONDISI 13

<img width="809" height="89" alt="Output Kondisi 13" src="https://github.com/user-attachments/assets/ac97dbf6-abb0-45f7-9c60-9ec5096a71b3" />


#Sistem Manajemen Daftar Barang Pinjaman

print("halaman Awal")

print("silahkan Login atau Mendaftar jika belum memiliki akun")

pilihan = input("Input Pilihan (Login/Mendaftar/Keluar): ")

if pilihan == "Login":

    print("Login")
    username = input("Input Username: ")
    password = input("Input Password: ")

    menu = input("Meminjam/Mengembalikan Barang?: ")
    if menu == "Meminjam":
        print("Silahkan Pilih Barang Yang Akan DiPinjam")

        barang = ["Mouse", "Keyboard", "Monitor"]
        print("barang")

        pinjam = input("Pilih(Mouse/Keyboard/Monitor): ")
        if pinjam == "Mouse":
            input("Input Tanggal Pemesanan: ")
            input("Input Tanggal Pengembalian: ")
            print("Peminjaman Barang Berhasil")
            barang.remove("Mouse")
            print("Barang Pinjaman Yang Tersedia", barang)

        elif pinjam == "Keyboard":
            input("Input Tanggal Pemesanan: ")
            input("Input Tanggal Pengembalian: ")
            print("Peminjaman Barang Berhasil")
            barang.remove("Keyboard")
            print("Barang Pinjaman Yang Tersedia", barang)

        elif pinjam == "Monitor":
                input("Input Tanggal Pemesanan: ")
                input("Input Tanggal Pengembalian: ")
                print("Peminjaman Barang Berhasil")
                barang.remove("Monitor")
                print("Barang Pinjaman Yang Tersedia", barang)

        else:
            print("Barang Tidak Ada/Tidak Tersedia")
    
    elif menu == "Mengembalikan":
        print("Silahkan Pilih Barang Yang Akan DiKembalikan")

        barang = ["Mouse", "Keyboard", "Monitor"]
        print("barang")

        mengembalikan = input("Pilih (Mouse/Keyboard/Monitor): ")
        if mengembalikan == "Mouse":
            barang.remove("Mouse")
            print("Barang Tersisa", barang)
            tanggal_1 = str(input("Input Tanggal Perjanjian Pengembalian: "))
            tanggal = str(input("Input Tanggal Pengembalian: "))
            if tanggal == tanggal_1:
                barang.append("Mouse")
                print("Pengembalian Barang Tepat Waktu, Barang Tersedia", barang)
            else:
                print("Pengembalain Barang Tidak Tepat Waktu, Barang Tersedia", barang)

        elif mengembalikan == "Keyboard":
            tanggal_1 = str(input("Input Tanggal Perjanjian Pengembalian: "))
            tanggal = str(input("Input Tanggal Pengembalian: "))
            if tanggal == tanggal_1:
                print("Pengembalian Barang Tepat Waktu")
            else:
                print("Pengembalain Barang Tidak Tepat Waktu")

        elif mengembalikan == "Monitor":
            tanggal_1 = str(input("Input Tanggal Perjanjian Pengembalian: "))
            tanggal = str(input("Input Tanggal Pengembalian: "))
            if tanggal == tanggal_1:
                print("Pengembalian Barang Tepat Waktu")
            else:
                print("Pengembalain Barang Tidak Tepat Waktu")

        else:
            print("Barang Tidak Termasuk")


elif pilihan == "Mendaftar":
    print("Mendaftar")
    email = input("Input Email: ")
    username = input("Input Username: ")
    password = input("Input Password: ")
    verifikasi = input("Apakah Verifikasi email Berhasil? (Ya/Tidak): ")
    if verifikasi == "Ya":
        print("Registrasi berhasil")

        print("Silahkan Pilih Barang Yang Akan DiPinjam")

        barang = ["Mouse", "Keyboard", "Monitor"]
        print("barang")

        pinjam = input("Pilih(Mouse/Keyboard/Monitor): ")
        if pinjam == "Mouse":
            input("Input Tanggal Pemesanan: ")
            input("Input Tanggal Pengembalian: ")
            print("Peminjaman Barang Berhasil")
            barang.remove("Mouse")
            print("Barang Pinjaman Yang Tersedia", barang)

        elif pinjam == "Keyboard":
            input("Input Tanggal Pemesanan: ")
            input("Input Tanggal Pengembalian: ")
            print("Peminjaman Barang Berhasil")
            barang.remove("Keyboard")
            print("Barang Pinjaman Yang Tersedia", barang)

        elif pinjam == "Monitor":
            input("Input Tanggal Pemesanan: ")
            input("Input Tanggal Pengembalian: ")
            print("Peminjaman Barang Berhasil")
            barang.remove("Monitor")
            print("Barang Pinjaman Yang Tersedia", barang)

        else:
            print("Barang Tidak Ada/Tidak Tersedia")
              

    else:
        print("Verivikasi Gagal, silahkan Mengulang")

elif pilihan == "Keluar":
    print("Keluar?")
    keluar = input("Ingin Keluar? (Ya/Tidak): ")
    if keluar == "Ya":
        print("Keluar dari halaman")
    else:
        print("Silahkan Pilih Login/Mendaftar")

else:
    print("Pilihan Salah/Tidak Ada")
