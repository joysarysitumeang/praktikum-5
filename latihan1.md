```python
# ================================
# Program Daftar Kontak (Dictionary)
# ================================

kontak = {
    "Ari": "0812678888",
    "Dina": "0876777776"
}

# Fungsi untuk menampilkan tabel kontak
def tampil_tabel():
    print("\nNama | Nomor Telepon")
    print("====================")
    for nama, nomor in kontak.items():
        print(f"{nama:<10} | {nomor}")


# Program menu
while True:
    print("\n=== MENU KONTAK ===")
    print("1. Tampilkan kontak Ari")
    print("2. Tambah kontak baru (manual)")
    print("3. Ubah nomor kontak (pilih manual)")
    print("4. Tampilkan semua Nama")
    print("5. Tampilkan semua Nomor")
    print("6. Tampilkan semua Nama dan Nomornya")
    print("7. Hapus kontak manual")
    print("8. Tampilkan TABEL Kontak")
    print("0. Keluar")

    pilihan = input("Pilih menu: ")

    # 1. Tampilkan Ari
    if pilihan == "1":
        print("\nKontak Ari:", kontak.get("Ari", "Tidak ditemukan"))

    # 2. Tambah kontak baru manual
    elif pilihan == "2":
        nama_baru = input("Masukkan nama kontak baru: ").strip()
        nomor_baru = input("Masukkan nomor telepon: ").strip()

        if nama_baru in kontak:
            print("Nama sudah ada! Gunakan menu ubah nomor jika ingin mengganti.")
        else:
            kontak[nama_baru] = nomor_baru
            print(f"Kontak {nama_baru} berhasil ditambahkan!")

    # 3. Ubah nomor manual
    elif pilihan == "3":
        print("\nDaftar kontak:")
        for nama in kontak:
            print("-", nama)

        nama_ubah = input("Pilih nama yang ingin diubah nomornya: ").strip()

        if nama_ubah not in kontak:
            print("Nama tidak ditemukan.")
        else:
            nomor_baru = input("Masukkan nomor baru: ").strip()
            kontak[nama_ubah] = nomor_baru
            print(f"Nomor {nama_ubah} berhasil diubah!")

    # 4. Tampilkan semua nama
    elif pilihan == "4":
        print("\nSemua Nama:")
        for nama in kontak.keys():
            print("-", nama)

    # 5. Tampilkan semua nomor
    elif pilihan == "5":
        print("\nSemua Nomor:")
        for nomor in kontak.values():
            print("-", nomor)

    # 6. Tampilkan semua daftar kontak
    elif pilihan == "6":
        print("\nDaftar Nama dan Nomor:")
        for nama, nomor in kontak.items():
            print(f"- {nama}: {nomor}")

    # 7. Hapus kontak manual
    elif pilihan == "7":
        print("\nDaftar kontak yang tersedia:")
        for nama in kontak:
            print("-", nama)

        nama_hapus = input("Masukkan nama kontak yang ingin dihapus: ").strip()

        if nama_hapus in kontak:
            del kontak[nama_hapus]
            print(f"Kontak {nama_hapus} berhasil dihapus!")
        else:
            print("Nama tidak ditemukan.")

    # 8. Tampilkan tabel
    elif pilihan == "8":
        tampil_tabel()

    # Keluar
    elif pilihan == "0":
        print("\nProgram selesai.")
        break

    else:
        print("Pilihan tidak valid, coba lagi.")
 ```
 # hasil output
<img width="1034" height="369" alt="Screenshot 2025-11-23 081952" src="https://github.com/user-attachments/assets/167d00d5-dc05-46a3-a54a-f1d5277bd74b" />
<img width="1122" height="396" alt="Screenshot 2025-11-23 082026" src="https://github.com/user-attachments/assets/a284af4a-61b9-497f-a74a-779da473a8c0" />
<img width="1137" height="496" alt="Screenshot 2025-11-23 082128" src="https://github.com/user-attachments/assets/770fe3c4-868f-483a-84c4-14f42aa8cf62" />
<img width="1114" height="449" alt="Screenshot 2025-11-23 082152" src="https://github.com/user-attachments/assets/365afe3c-0e1d-4918-b873-c4df9be84f52" />
<img width="1026" height="430" alt="Screenshot 2025-11-23 082205" src="https://github.com/user-attachments/assets/0be35fba-1565-459d-b7c0-e8b073a6d34d" />
<img width="1115" height="430" alt="Screenshot 2025-11-23 082223" src="https://github.com/user-attachments/assets/44bca089-9eca-43b8-9312-8f94580d4918" />
<img width="1101" height="481" alt="Screenshot 2025-11-23 082243" src="https://github.com/user-attachments/assets/c5abda94-0feb-4e53-9e17-de30e76ae4b7" />
<img width="1128" height="462" alt="Screenshot 2025-11-23 082306" src="https://github.com/user-attachments/assets/3f79588c-2c53-4ad4-8c19-70342c991aba" />








