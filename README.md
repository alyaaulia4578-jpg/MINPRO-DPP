# MINPRO-DPP
Alya Aulia - Sistem Informasi



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
