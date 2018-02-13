
# Oh My ZSH

## 1. Shell dan ZSH

**Shell** merupakan sebuah program penerjemah perintah yang memberikan jembatan antara user dengan kerel yang merupakan inti dari Sistem Operasi. Biasanya shell memiliki prompt sebagai user interface, yaitu tempat dimana user memberikan perintah-perintah yang diinginkan baik berupa perintah internal shell, ataupun perintah eksekusi suatu file progam.

**ZSH** adalah shell (command interpreter) dari keluarga shell Bourne, yang juga mencakup bash dan shell Korn (yang disebut zsh). Dikembangkan oleh Paul Falstad, zsh dimaksudkan untuk menjadi pengganti shell Bourne dan C.

## 2. Instalasi ZSH 
**Instalasi ZSH di Ubuntu** 
Membuka terminal dilinux, kemudian ketikan perintah di bawah ini 
```sh
$ sudo apt-get update
$ sudo apt-get install zsh
```
Setelah selesai menginstall, kita ganti default shell dari bash ke ZSH, dan pastikan sudah mere-boot komputer agar pergantian shell dapat di lakukan oleh komputer.
```sh
$ chsh -s /bin/zsh
$ sudo chsh -s /bin/zsh
$ sudo reboot
```
untuk mengecek shell yang aktif gunakan perintah di bawah ini
```sh
$ echo $SHELL
```
**Instalasi ZSH di MAC OS**

```sh
Instalasi ZSH dan Oh My ZSH pada Mac Dilakukan dalam satu command
```

## 3. Oh My ZSH
**Oh-My-Zsh** adalah framework open source, *community-driven* untuk mengelola konfigurasi ZSH. Muncul dibundel dengan banyak fungsi bermanfaat, pembantu, plugin, tema, dan beberapa hal lainnya.
## 4. Instalasi Oh My ZSH
**Instalasi Oh My ZSH via curl**
Ketikan perintah di bawah ini 
```sh
$ sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
**Instalasi Oh My ZSH Via wget** 
Ketikan perintah di bawah ini 
```sh
$ sh -c "$(wget https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
```
## 5. Mengganti Tema ZSH 
Pertama buka link di bawah ini, untuk memilih tema yang diinginkan 
> https://github.com/robbyrussell/oh-my-zsh/wiki/themes

Edit file `.zshrc` dengan cara mengetikan command dibawah ini 
```sh
$ nano .zshrc
```
Mengganti dengan nama tema yang diingin kan sesuai dengan list pada `ZSH_THEME = " "` yang di tulis didalam tanda petik `" "`
```sh
ZSH_THEME = "muse"
```
simpan dan keluar
## 6. Fitur ZSH yang tidak tersedia di Bash
ada beberapa fitus ZSH yang tidak tersedia di Bash, Diantaranya adalah :
 
- *Auto Correct* dalam mencari direktori
Misal, Kita mencari direktori ```Aplication``` dengan mengetikan command ```cd ap ``` maka akan mengkoreksi walaupun `a` yang di inputkan besar atau kecil
- *Auto completion* 
misal, apabila kita menginputkan hanya 'do' akan menglengkapi `document` atau `download`
- Menyediakan Alias untuk command populer, seperti :
1. ``` git status``` jadi ``` gst```
2. ``` ls -liah ``` jadi ```ll```
3. dll
- Bisa mengganti tema seperti pada nomer 5
