# wsl

## WSLでVS Codeを開く
.code

PowerShellまたはコマンドプロンプトで実行
wsl --list --verbose

または
wsl -l -v

例：Ubuntuを削除する場合
wsl --unregister Ubuntu
wsl --unregister AlmaLinux-9

特定のディストリビューション名で削除
wsl --unregister <ディストリビューション名>

利用可能なディストリビューションを確認
wsl --list --online

特定のディストリビューションをインストール
wsl --install -d Ubuntu
wsl --install -d AlmaLinux-9

または
wsl --install -d Ubuntu-22.04

WSLを完全にシャットダウン
wsl --shutdown

すべてのディストリビューションを確認して削除
wsl -l -v

各ディストリビューションに対して
wsl --unregister <名前>

WSLを再インストール
wsl --install

インストール済みのディストリビューション一覧を表示
wsl -l -v

WSLのバージョン情報を表示
wsl --version

インストール済みディストリビューションとそのWSLバージョンを表示
wsl -l -v

特定のディストリビューションをWSL2に変換
wsl --set-version Ubuntu-22.04 2

デフォルトのWSLバージョンを設定
wsl --set-default-version 2

特定のディストリビューションを起動
wsl -d Ubuntu-22.04
wsl -d Debian

デフォルトを変更
wsl --set-default Ubuntu-22.04

その後は単にwslコマンドで起動可能
wsl

利用可能なディストリビューション一覧を表示
wsl --list --online

特定のディストリビューションをインストール
wsl --install -d Ubuntu-20.04
wsl --install -d Debian
