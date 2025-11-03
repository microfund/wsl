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

### インストール済みディストリビューションの確認
```
PS C:\Users\user> wsl -l -v
  NAME           STATE           VERSION
* AlmaLinux-9    Running         2
```

### 利用可能なディストリビューションの確認
wsl --list --online

### 特定のディストリビューションを削除  
wsl --unregister <ディストリビューション名> 
wsl --unregister Ubuntu  
wsl --unregister AlmaLinux-9

### 特定のディストリビューションをインストール  
wsl --install -d Ubuntu  
wsl --install -d Ubuntu-22.04  
wsl --install -d Ubuntu-20.04  
wsl --install -d Debian  
wsl --install -d AlmaLinux-9

### WSLの完全シャットダウン
wsl --shutdown

### WSLの再インストール
wsl --install

### WSLバージョン情報の表示
wsl --version

### デフォルトのWSLバージョンを設定
wsl --set-default-version 2

### 特定のディストリビューションのWSLバージョンを変更
wsl --set-version Ubuntu-22.04 2

## ディストリビューションの起動

### 特定のディストリビューションを起動
wsl -d Ubuntu-22.04  
wsl -d Debian

### デフォルトディストリビューションの変更
wsl --set-default Ubuntu-22.04

### デフォルトディストリビューションの起動
wsl

## 完全リセット手順

1. すべてのディストリビューションを確認  
   wsl -l -v

2. 各ディストリビューションを削除  
   wsl --unregister <名前>

3. WSLを再インストール  
   wsl --install
