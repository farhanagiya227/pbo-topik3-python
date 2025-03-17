class Karyawan:
    def __init__(self, nama, jabatan):
        self.__nama = nama   # Private attribute
        self.__jabatan = jabatan  # Private attribute
    
    def bekerja(self):
        print(f"{self.__nama} sekarang bekerja sebagai {self.__jabatan}")
    
    def istirahat(self):
        print(f"{self.__nama} sekarang istirahat")
    
    # Getter untuk nama
    def get_nama(self):
        return self.__nama
    
    # Setter untuk nama
    def set_nama(self, nama_baru):
        self.__nama = nama_baru
    
    # Getter untuk jabatan
    def get_jabatan(self):
        return self.__jabatan
    
    # Setter untuk jabatan
    def set_jabatan(self, jabatan_baru):
        self.__jabatan = jabatan_baru

# Membuat objek karyawan
karyawan1 = Karyawan("Raka", "Manager")
karyawan2 = Karyawan("Sasa", "Staff")

# Objek baru
karyawan3 = Karyawan("Budi", "Supervisor")

# Akses variabel private menggunakan getter
print("Nama karyawan:", karyawan3.get_nama())  
print("Jabatan karyawan:", karyawan3.get_jabatan())

# Mengubah nilai private menggunakan setter
karyawan3.set_nama("Eka")
karyawan3.set_jabatan("Senior Supervisor")

# Menampilkan hasil perubahan
print("Nama karyawan setelah diubah:", karyawan3.get_nama())
print("Jabatan karyawan setelah diubah:", karyawan3.get_jabatan())
