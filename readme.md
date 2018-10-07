#GIT-FUNDAMENTAL
    
git adalah salah satu tool yang sering digunakan dalam projct pengembangan software

- mengetahui perintah dasar CLI

    - ls = list
        ```
        ls
        ```

    - cd = change directory (untuk masuk ke suatu direktori yang kita mau)

        masuk ke direktori
            ```
            cd Document/
            ```

        kembali ke direktori sebelumnya
            ```
            cd ../
            ```

        kembali ke default direktori (langsung masuk ke home)
            ```
            cd
            ```

    - pwd = print working direktori (untuk mengetahui di mana kita berada)
        ```
        pwd
        ```

    - touch = membuat file
        ```
        touch coba.txt (usahakan disertai dengan menggunakan extensi agar mudah dibaca)
        ```

    - mkdir = make direktori (untuk membuat direktori baru)
        ```
        mkdir folder
        ```

    - rmdir = remove direktori (untuk menghapus direktori)
        ```
        rmdir -r folder/
        ```
    
    - rm -r = remove (menghapus direktori beserta isinya)
        ```
        rm -r folder
        ```

- GITHUB
    
    - membuat akun github di link dibawah ini
        ```
        https://www.github.com
        ```

    - jika sudah  membuat akun kemudian membuat folder atau direktori yang kita mau untuk di kirim ke git
        ```
        mkdir coba
        ```

    - kemudian masuk ke dalam folder direktorinya dan membuat sebuah file bebas, contoh
        ```
        cd coba && touch coba .html
        ```

    - kemudian buka text editor untuk mengedit file 
        ```HTML
        coba.html
        ```

    - edit isi dari file tersebut dengan contoh :
        ```HTML
        <html>
            <head>
                <tittle>HAI TAYO</title>
            </head>
            <body>
                <h1>Hai Tayo</h1>
            </body>
        </html>
        ```

    - setelah selesai kemudian buka terminal dan masuk ke dalam folder kita
        ```
        cd folder
        ```

    - setelah itu kita inisialisasi folder yang akan kita git
        ```
        git init
        ```

    - setelah itu kita git add untuk bisa memasukan file kita kedalam repository  / ruang penyimpanan lokal
        ```
        git add <nama file>
        ```
        atau untuk langsung bisa memasukan banyak file dengan
        ```
        git add .
        ```

    - untuk mengetahui status dari file kita apakah sudah ke add belum dengan cara
        ```
        git status
        ```
    !! apabila berwarna hijau berrti sudah ke add kedalam tepo lokal apabila merah berarti belum ke add kedalam repo lokal !!

    - kemudian git commit untuk memberikan komentar di file kita agar ita tahu kenapa file kita di git
        ```
        git commit -m "<nama coment>"
        ```
    - kemudian membuat repository di github kita sendiri
    - kemudian ikuti langkah" di repo github yang telah kalian buat
        - add readme.md
            ```
            echo coba >> "readme.md"
            ```

        - cek status dari file readme kita
            ```
            git status
            ```
        
        - remote file git kita untuk bisa terarah ke github kita sendiri
            ```HTML
            git remote add origin https://<link dari github kita tadi>
            ```
        
        - setelah itu push/upload file kita
            ```
            git push -u origin master
            ```

        - jika sudah selesai refresh link repo kita sendiri, maka kalian akan melihat file yang telah kalian push/upload tadi

# Cara Kontribute di repo orang lain
keunggulan git salah satuya adalah kita bisa berkontribusi pada repo orang atau ikut berkontribusi pada sebuah project yang kita mau denan seizin pemilik repo tersebut.

- klick menu forks yang ada di pojok kanan atas

- kita clone terlebih dahulu repo orang lain
    ```git
    git clone https://github.com/<repo yang ingin di clone>
    ```

- setelah kita clone kita update project tersebut dengan
    ```
    git pull https://github.com/<repo yang mau di update>
    ```

- setelah di update kita push ke dalam repo kita supaya bisa menjadi repo milik kita sendiri
    ```git
    git push -u origin master
    ```

    ```
    -> jika kita ingin salah melakukan pengeditan pada file pull kita, kita tidak perlu kawatir, kita tinggal pull lagi repo tadi <-
        -> dengan git pull
        ```
        git pull https://github.com/<repo yang tadi untuk di update> <-
        ```
    ```

- jika sudah kita buat file baru atau edit beberapa bagian di file yang telah kita pull tadi

- jika sudah kita add dan kita commit file kita tadi untuk bisa di kirim ke github
    ```
    git add <nama file> && git commit -m "nama coment"
    ```

- jika sudah ki pindah ke menu pull request
    >!! untuk pull request kita lakukan pada repo kita sendiri bukan pada repo orang lain !!
    
- jika sudah di klick new pull request kita tinggal tunggu sampai si pemilik project supaya bisa di terima pull request kita

- jika sudah kita update lagi repo yang baru
    ```
    git pull https://github.com/<repo tujuan>
    ```

- setelah itu kita push kembali ke repo kita
    ```
    git push -u origin master
    ```