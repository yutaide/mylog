# PX4\_Firmware

px4\_firmwareのcommitにtagが付けられていないと「makeコマンドでビルドしてgazebo起動」の際にエラーが出てしまう。  
upstream側をforkした時にtagも含めておく必要があった。忘れていた場合は、以下のようにしてtagをfetchしてくる。

```text
# リポジトリのremote確認
git remote -v

# upstreamをremoteに追加
git remote add upstream https://github.com/PX4/Firmware.git

# tagをfetch
git fetch --all

# tagをorigin(forkした側のリポ)にpush
git push origin --tags
```



