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

