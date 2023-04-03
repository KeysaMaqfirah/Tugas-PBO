# Contoh program dengan pendekatan fungsional programming

# Fungsi untuk menghitung total harga setelah diskon
def total_harga(diskon, *harga):
    diskon_harga = map(lambda harga: harga * (1-diskon), harga)
    return sum(diskon_harga)

# Memanggil fungsi
diskon = 0.2
harga = [1000, 2000, 3000, 4000]
final_harga= total_harga(diskon, *harga)
print(final_harga) # 8000.0

# Membuat kelas untuk produk
class Produk:
    def __init__(self, nama_barang, harga_barang):
        self.nama_barang = nama_barang
        self.harga_barang = harga_barang

    def get_harga(self, diskon_barang):
        return self.harga_barang * (1 - diskon_barang)
        
        
        

# Contoh OOP pada Python :

# Membuat kelas untuk produk
class Produk:
    def __init__(self, nama_barang, harga_barang):
        self.nama_barang = nama_barang
        self.harga_barang = harga_barang

    def get_harga(self, diskon_barang):
        return self.harga_barang * (1 - diskon_barang)

# Membuat kelas untuk keranjang belanja
class Belanja:
    def __init__(self):
        self.items = []

    def add_item(self, produk):
        self.items.append(produk)

    def total_harga(self, diskon_harga):
        return sum([item.get_harga(diskon_harga) for item in self.items])

# Membuat objek produk dan keranjang belanja
produk1 = Produk("Buku", 2000)
produk2 = Produk("Pensil", 2000)
keranjang = Belanja()

# Menambahkan produk ke keranjang
keranjang.add_item(produk1)
keranjang.add_item(produk2)

# Menghitung total harga
diskon_harga = 0.1
final_harga = keranjang.total_harga(diskon_harga)
print(final_harga) # 3600.0

