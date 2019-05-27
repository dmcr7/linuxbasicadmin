#### Linux Basic Admin:

##### list

Menampilkan list detail

          ls -l

Menampilkan list keseluruhan (termasuk dot file)

          ls -la

Menampilkan list berdasarkan waktu

          ls -t

Menampilkan list berdasarkan ukuran file

        ls -S

Menampilkan list berdasarkan tipe file

        ls -F

Menampilkan list dengan index file nya

        ls -i


##### cat
Print ke terminal isi dari file

        cat [ file ]

##### Mengubah directori

Mengubah directori folder

      cd

##### Tail
Menampilkan baris akhir sebanyak n

      [perintah lain] | tail -n

Monitoring perubahan file

      tail -f [nama file]

##### Head
Menampilkan baris awal sebanyak n

      [perintah lain] | head -n

##### Right Direction
Replace isi dari file output

      cat /proc/cpuinfo > command.txt

##### Double Right DirectionInsert sesuatu pada file output

      cat /proc/cpuinfo | wc -l >> command.txt

##### Left Direction
File sebagai input (yang diproses)

      ./program < command.txt

##### Error Direction
Memasukkan error pada file output

        mkdir Music 2> myerror.txt (replace)
        mkdir Music 2>> myerror.txt (insert)

##### Sort
Mengurutkan isi file (per baris)

        sort -u [namafile]

##### Uniq
Menghitung jumlah elemen per nilai dalam data

        uniq -c [namafile]

##### Grep
Mencari kata dalam suatu file

        [perintah] | grep [keyword]

##### Copy
Copy semua file dalam satu direktori

        cp * [direktori tujuan]

Copy semua file dan sub direktori

        cp -R * [direktori tujuan]

Copy file

        cp [namafile] [direktori tujuan]

Copy tanpa merubah date timestamps

        cp -p

##### Move
Jika belum ada nama, membuat file baru. Jika sudah ada nama, memindahkan

        mv

##### SSH
Komputer A SSH komputer B

        ssh B@ip

A kirim file ke B

        scp [nama file] B@ip:direktori

B mengambil file dari A

        scp A@ip:direktori [direktori lokal]

SSH tanpa password

        sshpass -p [password]

ssh dengan perintah

        A@ip [perintah]

##### Create New File
Membuat file baru

        touch [nama file]

##### Check Direction
Menampilkan alamat direktori aktif

        pwd

##### Locate
Mencari file pada semua direktori

      locate [keyword]

##### Find
Mencari file pada direktori aktif

      Find [keyword]

##### Remove
Menghapus folder yang kosong

      rmdir

Menghapus file

      rm [direktori file]

Menghapus semua isi direktori

      rm -r [direktori]

Menghapus Paksa semua isi dir (force)

      rm -rf [file / dir]

##### Check IP Address
Mengecek IP Addres

      ifconfig
      ip address

##### Show Process
Untuk melihat process status

      ps -ef

##### Check env
Print Environment Variable

      env

##### Displays and updates sorted process information
Menampilkan process secara update dan terurut

      top
      htop

##### Shows the network status
Menampilkan status network

      netstat

##### Display free disk space
Menampilkan disk space yang bisa dipakai

      df -h

-h prints out the information in human-readable format

##### To check the user running the application
Melihat user id yang berjalan

      id

##### Change permision
Mengubah permision suatu File

      chmod [parameter] [file]

contoh : chmod +x bash.sh, chmod 777 bash.sh

##### dig/nslookup
dig (DNS lookup utility) or nslookup (query Internet name servers)

      dig equnix.asia
      nslookup equnix.asia

##### history
melihat history command

      history
