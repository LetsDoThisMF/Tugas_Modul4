import Method
nol = 0
Budget = 1000000000

print("Budget anda: ", Budget)
print("Selamat datang di toko 41 computer\n")

def listmerek():
    print("""
    Persiapkan uang belanja anda!
     list kode, laptop, dan harganya
    1 : asus\t     - Rp. 10.000.000
    2 : lenovo\t\t - Rp.  8.000.000
    3 : advan\t    - Rp.  7.000.000
    4 : hp\t\t     - Rp.  9.000.000
    5 : acer\t\t   - Rp.  11.000.000
    0 : Batal
    """)

def opsimerek(opsi):
    switcher = {
        1: "asus \t - Rp. 10.000.000",
        2: "lenovo \t - Rp. 8.000.000",
        3: "advan \t - Rp. 7.000.000",
        4: "hp \t - Rp. 9.000.000",
        5: "acer \t - Rp. 11.000.000",
        0: "Program selesai",
    }

    return switcher.get(opsi, "Kode tersebut salah")

def hargamerek(opsi):
    if opsi == 1:
        harga = 10000000
    elif opsi == 2:
        harga = 8000000
    elif opsi == 3:
        harga = 7000000
    elif opsi == 4:
        harga = 9000000
    elif opsi == 5:
        harga = 11000000
    else:
        print("Opsi anda salah! ")
        return
    return harga

def totalModal():
    total = 0
    while True:
        listmerek()
        m = int(input("Masukkan kode merek laptop : "))
        print(opsimerek(m))
        list = [opsimerek(m)]
        q = int(input("Masukkan jumlah laptop yang ingin anda beli : "))
        totalAwal = hargamerek(m) * q
        total += totalAwal
        print("Total harga belanja anda : ", total)
        belilagi = int(input("Apakah anda masih ingin membeli laptop lagi? : (1. Iya/ 0. Tidak) : "))
        if belilagi != 1:
            print("Total harga belanja anda  : ", total)
            break

    return total

def diskon(totalBayar):
    if totalBayar > 30000000:
        totalBayar *= 0.75  # diskon 25%
    elif totalBayar > 25000000:
        totalBayar *= 0.90  # diskon 10%
    elif totalBayar > 18000000:
        totalBayar *= 0.95  # diskon 5%
    return totalBayar

total = totalModal()
panggil = Method.Method(total)
print("total harga dengan diskon : ", diskon(total))
print("Sisa budget anda: ", Budget - int(diskon(total)))
panggil.trims()
panggil.selesai(5)
input("ENTER untuk selesai")
