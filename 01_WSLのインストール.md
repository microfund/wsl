
# 🐧 WSL Guide (Windows Subsystem for Linux)

*WSLの使い方ガイド（Windows Subsystem for Linux）*

---

## 📚 Table of Contents | 目次

* [Introduction | はじめに](#introduction--はじめに)
* [How to Use WSL | WSLの使い方](#how-to-use-wsl--wslの使い方)

  * [Start WSL | WSLを起動する](#start-wsl--wslを起動する)
  * [Move from Windows to Linux | WindowsからLinuxへ移動する](#move-from-windows-to-linux--windowsからlinuxへ移動する)
  * [Open VS Code in WSL | WSLでVS Codeを開く](#open-vs-code-in-wsl--wslでvs-codeを開く)
  * [Check Installed OS | インストール済みOSを確認する](#check-installed-os--インストール済みosを確認する)
  * [List Available OS | インストール可能なOSを確認する](#list-available-os--インストール可能なosを確認する)
  * [Unregister Distribution | 特定のディストリビューションを削除](#unregister-distribution--特定のディストリビューションを削除)
  * [Install Distribution | 特定のディストリビューションをインストール](#install-distribution--特定のディストリビューションをインストール)
  * [Shutdown WSL | WSLの完全シャットダウン](#shutdown-wsl--wslの完全シャットダウン)
  * [Reinstall WSL | WSLの再インストール](#reinstall-wsl--wslの再インストール)
  * [Show Version Info | WSLバージョン情報の表示](#show-version-info--wslバージョン情報の表示)
  * [Set Default Version | デフォルトのWSLバージョンを設定](#set-default-version--デフォルトのwslバージョンを設定)
  * [Change WSL Version | 特定のディストリビューションのWSLバージョンを変更](#change-wsl-version--特定のディストリビューションのwslバージョンを変更)
* [Run Distribution | ディストリビューションの起動](#run-distribution--ディストリビューションの起動)

  * [Launch Specific Distribution | 特定のディストリビューションを起動](#launch-specific-distribution--特定のディストリビューションを起動)
  * [Change Default Distribution | デフォルトディストリビューションの変更](#change-default-distribution--デフォルトディストリビューションの変更)
  * [Launch Default Distribution | デフォルトディストリビューションの起動](#launch-default-distribution--デフォルトディストリビューションの起動)
* [Reset WSL | 完全リセット手順](#reset-wsl--完全リセット手順)
* [License | ライセンス](#license--ライセンス)

---

## Introduction | はじめに

This repository explains how to manage and use **WSL (Windows Subsystem for Linux)** on Windows.
このリポジトリは、WindowsでWSLを使うための基本操作をまとめたガイドです。

---

## How to Use WSL | WSLの使い方

### Start WSL | WSLを起動する

```powershell
PS C:\Users\user> wsl
```

### Move from Windows to Linux | WindowsからLinuxへ移動する

```bash
$ cd ~
```

### Open VS Code in WSL | WSLでVS Codeを開く

```bash
code .
```

### Check Installed OS | インストール済みOSを確認する

```powershell
wsl -l -v
```

### List Available OS | インストール可能なOSを確認する

```powershell
wsl --list --online
```

### Unregister Distribution | 特定のディストリビューションを削除

```powershell
wsl --unregister <ディストリビューション名>
```

### Install Distribution | 特定のディストリビューションをインストール

```powershell
wsl --install -d Ubuntu-22.04
```

### Shutdown WSL | WSLの完全シャットダウン

```powershell
wsl --shutdown
```

### Reinstall WSL | WSLの再インストール

```powershell
wsl --install
```

### Show Version Info | WSLバージョン情報の表示

```powershell
wsl --version
```

### Set Default Version | デフォルト
