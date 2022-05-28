#Input
pembeli=input("Input Nama Pembeli : ")
no_hp=input("Input No. Handphone : ")
jenis=input("Input Jenis Baju [A/R/D] : ")
#Proses
if jenis=="A":
    jenisbaju="Anak"
    harga=30000
elif jenis=="R":
    jenisbaju="Remaja"
    harga=70000
else :
    jenisbaju="Dewasa"
    harga=100000

#Input Jumlah Beli
jumlah=int(input("Masukan Jumlah Beli : "))

#Proses Potongan
if jumlah>=2 :
    potongan=(jumlah*harga)*0.10
else:
    potongan=0

total=(jumlah*harga)-potongan

#Cetak Hasil
print("----------------------------")
print("        Toko Baju Moderna")
print("  Jam operasional 08.00-21.00")
print("Jl.Raya Cikarang-Cibarusah No.168")
print("----------------------------")
print("Nama Pembeli : "+str(pembeli))
print("No. Handphone : "+str(no_hp))
print("Kode Jenis yang dipilih : "+str(jenis))
print("Nama Jenis Baju : "+str(jenisbaju))
print("harga : ",+(total))
print("Jumlah Beli :",+(jumlah))
ubay=int(input("Masukan Uang Bayar : "))
uangkembali=ubay-total
print("Uang Kembali : ",+uangkembali)
