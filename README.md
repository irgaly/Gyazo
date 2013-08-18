# Gyazogle

Copyright (c) 2013 irgaly.
This software is licensed under the GPL.

This software is forked version of [Gyazo](https://github.com/gyazo/Gyazo).

Google Picasa 版の Gyazo 。 Picasa の指定のアルバムへスクリーンショットをアップロードします。

動作には [GoogleCL](https://code.google.com/p/googlecl/) が必要です。

### GoogleCLのインストール(Homebrew)

* brew install python
* pip install googlecl
* 事前にgoogleコマンドでログインしておく

```bash
% google picasa list-albums
Please specify user: [google user name]
dyld: DYLD_ environment variables being ignored because main executable (/usr/bin/osascript) is code signed with entitlements
Please log in and/or grant access via your browser at https://www.google.com/accounts/OAuthAuthorizeToken?oauth_token=.......&hd=default then hit enter. [Enter]
```

### Path の設定

Gyazogle は ruby と googlecl コマンドが必要です。
デフォルトでは Mac 標準の /usr/bin/ruby と Homebrew からインストールされた /usr/local/bin/google を参照します。
設定ファイルを設置することで別の箇所へインストールされたコマンドを使用することが可能です。

次の内容の plist ファイルを ~/Library/Preferences/net.irgaly.gyazogle.plist へ設置してください。

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
  <key>ruby-path</key>
  <string>/usr/bin/ruby</string>
  <key>googlecl-path</key>
  <string>/usr/local/bin/google</string>
</dict>
</plist>
```

