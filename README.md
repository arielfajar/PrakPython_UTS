# PrakPython_UTS

Aplikasi Sederhana Menggunakan CRUD dan mysql-connector

Di dalam Aplikasi ini ada beberapa fungsi program, diantaranya :

1. Insert Data = untuk menambahkan data stok barang
        
        #Rumus untuk mencari stok_akhir
        stok_akhir = stok_awal + barang_masuk - barang_keluar
        
        #mencetak Stok_Akhir dari rumus sebelumnya
        print("stok akhir : ", stok_akhir)
        
        insert_data(id_barang, nama_barang, harga_barang, stok_awal, barang_masuk, barang_keluar, stok_akhir)
        
2. Show Data = untuk menampilkan data
				
		elif menu == "2":
			show_data()
        
3. Update Data = untuk mengupdate data berdasarkan id_barang
        
        stok_akhir = stok_awal + barang_masuk - barang_keluar
        print("stok akhir setelah diupdate : ", stok_akhir)
        
        update_data(id_barang, nama_barang, harga_barang, stok_awal, barang_masuk, barang_keluar, stok_akhir)
        
4. Hapus Data = untuk menghapus data berdasarkan id_barang
				
	 	elif menu == "4":
				
		id_barang = input("Masukkan id barang yang ingin dihapus : ")
		delete_data(id_barang)
        
5. Cari Data = untuk mencari data berdasarkan id_barang

		elif menu == "5":
  		id_barang = input("Masukkan id barang yang ingin dicari : ")
        
     	search_data(id_barang)
        
6. Keluar

		elif menu == "6":
    	print("Terima kasih sudah menggunakan Layanan Aplikasi Kami")
     	break

Program ini menggunakan loop while True, sehingga pengguna dapat memilih menu yang diinginkan selama program belum diakhiri (menu 6). Setelah pengguna memilih menu, program akan meminta input sesuai dengan fungsi yang dipilih dan kemudian menjalankan fungsi yang diinginkan. Setiap fungsi akan mengakses database MySQL yang dihubungkan dengan program menggunakan library mysql.connector dan melakukan operasi yang diinginkan. Setelah operasi selesai, program akan mengeluarkan pesan bahwa operasi telah berhasil dilakukan
