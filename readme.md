#GIT-FUNDAMENTAL
    
git adalah salah satu tool yang sering digunakan dalam projct pengembangan software

- mengetahui perintah dasar CLI

    ls = list
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
    
    - rm -r = remove (menghapus direktori beserta isinyas)
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
            cd coba
        ```
            ```
            touch coba .html
        ```

    - kemudian buka text editor untuk mengedit file 
            ```
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
                ```
                git remote add origin https://<link dari github kita tadi>
            ```
        
        - setelah itu push/upload file kita
                ```
                git push -u origin master
            ```