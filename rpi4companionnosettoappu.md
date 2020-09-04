# RPI4\(companion\)のセットアップ手順

raspios-liteをsdカードに書き込み、RPI4に差し込んで起動。

sudo dpkg-reconfigure keyboardなんとかでキー配置を日本語に対応させる。

セットアップ用スクリプトを入れたusbをマウントして、該当スクリプトをRPI4にコピー。

```text
# usb接続前に実行
ls /dev/sd*

# usb接続後に実行.接続前の出力との差をみてusbの認識がどこなのか確認
# /dev/sda /dev/sda1のように出たら数字がついている/dev/sda1を優先
ls /dev/sd*

# /mediaとしてマウントする
(例)sudo mount -t vfat /dev/sda1 /media

# cd /mediaでアクセスできる
# アンマウントは以下のとおり
(例)sudo umount /media
```

スクリプトを実行してrosをインストール。

mavrosインストール用スクリプトのUSER\_HOME\_DIRを自分の環境に合わせてから、スクリプトを実行してmavrosをインストール。\(一緒にmavlink等もインストールされる。\)

```text
# たとえばUSER_HOME_DIRが以下のようになっている
USER_HOME_DIR=/root

# ラズパイでユーザーがpiの場合は以下のように変更してからスクリプトを実行する
USER_HOME_DIR=/home/pi
```



