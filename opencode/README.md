# opencodeの設定ファイル

このディレクトリ配下の`opencode`ディレクトリを`~/.config/opencode`にシンボリックリンクしてください。

## Linux/macOS

```shell
ln -s $(pwd)/opencode ~/.config/opencode
```

## Windows (未検証)

```powershell
New-Item -ItemType Directory -Path $env:USERPROFILE\.config
New-Item -ItemType SymbolicLink -Path $env:USERPROFILE\.config\opencode -Target (Join-Path (Get-Location) "opencode")
```

## アプリケーション推論プロファイルを使う場合

`$.provider.amazon-bedrock.models` のキーにアプリケーション推論プロファイルのARNを設定します。

ただし、環境変数 `AWS_REGION` と使用するアプリケーション推論プロファイルのリージョン名を合わせておく必要があります。

```shell
export AWS_REGION=us-west-2

# opencode.json の $.provider.amazon-bedrock.models のキー
arn:aws:bedrock:us-west-2:{env:AWS_ACCOUNT_ID}:application-inference-profile/{env:GPT_OSS_20B_APPLICATION_PROFILE_ID}
```

## Links

- [opencode](https://opencode.ai/)
- [GitHub - sst/opencode: opencode](https://github.com/sst/opencode)
- [VS Code extension for opencode](https://marketplace.visualstudio.com/items?itemName=sst-dev.opencode)
