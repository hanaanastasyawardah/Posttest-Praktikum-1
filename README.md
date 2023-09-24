# Fungsi untuk menghitung volume bola
def hitung_volume_bola(r):
    return (4/3) * 3.14 * r**3

# Fungsi untuk menghitung volume tabung
def hitung_volume_tabung(r, t):
    return 3.14 * r**2 * t

# Fungsi untuk menghitung volume limas segitiga
def hitung_volume_limas_segitiga(luas_alas, t):
    return (1/3) * luas_alas * t

# Input nama dan NIM
nama = input("Masukkan nama: ")
nim = input("Masukkan NIM: ")

# Menampilkan menu pilihan
print("Pilih bangun ruang:")
print("1. Bola")
print("2. Tabung")
print("3. Limas Segitiga")

# Meminta pengguna memilih
pilihan = int(input("Masukkan nomor pilihan (1/2/3): "))

# Mengecek pilihan pengguna
if pilihan == 1:
    r = float(input("Masukkan jari-jari bola: "))
    volume = hitung_volume_bola(r)
    print(f"Volume bola dengan jari-jari {r} adalah {volume}")
elif pilihan == 2:
    r = float(input("Masukkan jari-jari tabung: "))
    t = float(input("Masukkan tinggi tabung: "))
    volume = hitung_volume_tabung(r, t)
    print(f"Volume tabung dengan jari-jari {r} dan tinggi {t} adalah {volume}")
elif pilihan == 3:
    luas_alas = float(input("Masukkan luas alas limas segitiga: "))
    t = float(input("Masukkan tinggi limas segitiga: "))
    volume = hitung_volume_limas_segitiga(luas_alas, t)
    print(f"Volume limas segitiga dengan luas alas {luas_alas} dan tinggi {t} adalah {volume}")
else:
    print("Pilihan tidak valid")

# Menampilkan nama dan NIM
print(f"Nama: {nama}")
print(f"NIM: {nim}")

Output:

PS C:\Users\asus\Downloads> & C:/Users/asus/AppData/Local/Programs/Python/Python311/python.exe "c:/Users/asus/Downloads/# Fungsi untuk menghitung volume bola.py"
Masukkan nama: hana anastasya wardah
Masukkan NIM: 12
Pilih bangun ruang:
1. Bola
2. Tabung
3. Limas Segitiga
Masukkan nomor pilihan (1/2/3): 2
Masukkan jari-jari tabung: 8
Masukkan tinggi tabung: 12
Volume tabung dengan jari-jari 8.0 dan tinggi 12.0 adalah 2411.52
Nama: hana anastasya wardah
NIM: 12
PS C:\Users\asus\Downloads>
