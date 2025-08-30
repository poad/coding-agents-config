# Claude Codeの設定ファイル

このディレクトリ配下の`.claude`ディレクトリを`~/.claude`にシンボリックリンクしてください。

## Linux/macOS

```shell
ln -s $(pwd)/.claude ~/.claude
```

## Windows

```powershell
New-Item -ItemType SymbolicLink -Path $env:USERPROFILE\.claude -Target (Join-Path (Get-Location) '.claude')
```

## Links

- [Claude](https://claude.ai/)
