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

## Links

- [opencode](https://opencode.ai/)
- [GitHub - sst/opencode: opencode](https://github.com/sst/opencode)
- [VS Code extension for opencode](https://marketplace.visualstudio.com/items?itemName=sst-dev.opencode)
