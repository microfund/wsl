## WSLの使い方 (Windows Subsystem for Linux) 

### WSLを起動する
1. PowerShellを起動する
2. wslとコマンドを打つ
```
PS C:\Users\user> wsl
```

### windowsからlinuxへ移動する
```
$ cd ~
```

### WSLでVS Codeを開く
```
code .
```

### インストール済みのOSを確認する
```
PS C:\Users\user> wsl -l -v
  NAME           STATE           VERSION
* AlmaLinux-9    Running         2
```

### インストール可能なOSを確認する
```
PS C:\Users\user> wsl --list --online

NAME                            FRIENDLY NAME
AlmaLinux-8                     AlmaLinux OS 8
AlmaLinux-9                     AlmaLinux OS 9
AlmaLinux-Kitten-10             AlmaLinux OS Kitten 10
AlmaLinux-10                    AlmaLinux OS 10
Debian                          Debian GNU/Linux
FedoraLinux-43                  Fedora Linux 43
FedoraLinux-42                  Fedora Linux 42
SUSE-Linux-Enterprise-15-SP6    SUSE Linux Enterprise 15 SP6
SUSE-Linux-Enterprise-15-SP7    SUSE Linux Enterprise 15 SP7
Ubuntu                          Ubuntu
Ubuntu-24.04                    Ubuntu 24.04 LTS
archlinux                       Arch Linux
kali-linux                      Kali Linux Rolling
openSUSE-Tumbleweed             openSUSE Tumbleweed
openSUSE-Leap-16.0              openSUSE Leap 16.0
Ubuntu-20.04                    Ubuntu 20.04 LTS
Ubuntu-22.04                    Ubuntu 22.04 LTS
OracleLinux_7_9                 Oracle Linux 7.9
OracleLinux_8_10                Oracle Linux 8.10
OracleLinux_9_5                 Oracle Linux 9.5
openSUSE-Leap-15.6              openSUSE Leap 15.6
```

### 特定のOSをインストールする  
```
wsl --install -d AlmaLinux-9
wsl --install -d Ubuntu-22.04  
wsl --install -d Ubuntu-20.04  
wsl --install -d Debian  
```

### 特定のOSを削除する
```
wsl --unregister <OS名> 
wsl --unregister AlmaLinux-9
```

### WSLをシャットダウンする
```
wsl --shutdown
```

### WSLの再インストール
```
wsl --install
```

### WSLバージョン情報の表示
```
wsl --version
```

### デフォルトのWSLバージョンを設定
```
wsl --set-default-version 2
```

### 特定のOSのWSLバージョンを変更
```
wsl --set-version Ubuntu-22.04 2
```



### 特定のOSを起動
```
wsl -d Ubuntu-22.04  
wsl -d Debian
```

### OSの変更
```
wsl --set-default Ubuntu-22.04
```

### デフォルトOSの起動
```
wsl
```

### 完全リセット手順
```
wsl -l -v
wsl --unregister <名前>
wsl --install
```
  
