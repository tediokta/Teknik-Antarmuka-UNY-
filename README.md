# Judul Praktikum

Interfacing Laboratory (Teknik Antarmuka)

## Deskripsi

Program Antarmuka dengan VS Code dan bahasa C++
* Download VS Code disini (https://code.visualstudio.com/download)
* Download MinGW-x64 disini (https://github.com/msys2/msys2-installer/releases/download/2024-12-08/msys2-x86_64-20241208.exe)

## Langkah-Langkah
1) Download, install, dan jalankan Visual Studio Code.
2) Pilih ikon ekstensi.
3) Cari "C++".
4) Pilih install.
   ![alt text](https://github.com/tediokta/Teknik-Antarmuka-UNY-/blob/2b783f8636c79c51f3bdc32a25711a916f614bfa/cpp-extension.png)

5) Download dan jalankan MinGW-x64

   ![alt text](https://github.com/tediokta/Teknik-Antarmuka-UNY-/blob/2b783f8636c79c51f3bdc32a25711a916f614bfa/MSYS2.png)

6) Pada installer, pilih folder instalasi yang diinginkkan dan catat (disarankan menggunakan direktori yang direkomendasikan)
7) Setelah selesai instalasi, pastikan kotak Run MSYS2 now tercentang dan pilih "Finish". Terminal MSYS2 otomatis akan terbuka.
8) Pada terminal ketikkan kode berikut "pacman -S --needed base-devel mingw-w64-ucrt-x86_64-toolchain"
9) Tekan Enter kemudian ketik "Y"
   ![alt text](https://github.com/tediokta/Teknik-Antarmuka-UNY-/blob/2b783f8636c79c51f3bdc32a25711a916f614bfa/cpp-install-msys2-toolchain.png)
10) Tambahkan path MinGW-w64 bin folder ke Windows PATH environment variable dengan menggunakan langkah berikut:
    *  Pada windows search bar ketik "Edit environment"
    *  Pada variabel User, pilih variable Path dan pilih Edit
       ![alt text](https://github.com/tediokta/Teknik-Antarmuka-UNY-/blob/2b783f8636c79c51f3bdc32a25711a916f614bfa/Env_User.png)
    *  Pilih New dan tambahkan folder destinasi MinGW-w64 yang sudah Anda cata pada proses instalasi ke dalam list. Path defaultnya adalah C:\msys64\ucrt64\bin
    *  Pilih OK kemudian OK kembali
11) Cek apakah MinGW-w64 tools sudah terinstall dengan benar dan tersedia, buka Command Prompt baru dan ketikkan:
   *	gcc --version
   *	g++ --version
   *	gdb --version
12.	Masih pada Command Prompt, buat sebuah file C++ baru dengan mengetikkan:
   *	mkdir projects
   *	cd Teknik Antarmuka
   *	code .
14) Buat file baru dengan nama "helloworld.cpp" dengan ikon "New File pada File Explorer atau File > New File command
    ![alt text](https://github.com/tediokta/Teknik-Antarmuka-UNY-/blob/2b783f8636c79c51f3bdc32a25711a916f614bfa/new-file.png)
   
15) Tes Program, ketikkan baris kode berikut:
      #include <iostream>
      int main()
       {
      std::cout << "Hello World" << std::endl;
       }
17) Simpan kode program dengan "Ctrl + S"
18) Klik tombol play di pojok kanan atas
    ![alt text](https://github.com/tediokta/Teknik-Antarmuka-UNY-/blob/2b783f8636c79c51f3bdc32a25711a916f614bfa/run-play-button.png)
 
19) Pilih "C/C++: g++.exe build and debug active file" dari list compiler yang terdeteksi pada sistem.
    ![alt text](https://github.com/tediokta/Teknik-Antarmuka-UNY-/blob/2b783f8636c79c51f3bdc32a25711a916f614bfa/select-gcc-compiler.png)
   
20) Apabila berhasil makan akan muncul tulisan "Hello World" pada terminal.
