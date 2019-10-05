# rubyshell

【 技術的な環境構築のための実験的コンテナ 】

[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](LICENSE)![GitHub release](https://img.shields.io/github/release/takkii/rubyshell.svg?style=flat)

※rubyshellの部分は、ビルド名で任意です

[ 起動 ]

```ruby
# clone
git clone https://github.com/takkii/rubyshell.git

# move
cd rubyshell

# build
docker build -t rubyshell .

# run
docker run -it rubyshell /bin/bash
```

[ コンテナ試運転 ]

```ruby
# etc
gem install zinbei

# read
source ~/.bashrc

# zinbei run

zinbei -h

or

zinbeiw
```

[ 環境...明記は初期、以降はGitHubリリース参照 ]

```markdown
ubuntu 18.04

git + rbenv + ruby-build

ruby 2.6.5 (+JIT)

rails 6.0.0
```

[ 動作環境確認 & ライセンス & 作成者 ]

```markdown
動作確認

Windows10 powershell & WSL
MacOS mojave

rubyshellはMITライセンスです

作成者 Takauki.K
```

> ※ フォルダを作り、Dockerfileは開発用途にわけて更新します。
