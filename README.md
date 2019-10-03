# rubyshell

【 技術的な環境構築のための実験的コンテナ 】

[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](LICENSE)![GitHub release](https://img.shields.io/github/release/takkii/rubyshell.svg?style=flat)

とりあえず試すときに使う環境

使い方 ( rubyshellの部分は、ビルド名で任意です )

```ruby
# move
cd rubyshell

# build
docker build -t rubyshell .

# run
docker run -it rubyshell /bin/bash
```

試す

```ruby
# etc
gem install zinbei

# read
source ~/.bashrc

# zinbei run
zinbei -v

or

zinbei -d
zinbei -s
zinbei -h

...etc

zinbeiw

```

環境

```markdown
ubuntu 18.04

git + rbenv + ruby-build

ruby 2.6.5 (+JIT)

rails 6.0.0
```

License & Author

```markdown
MITライセンスです

作成者 Takauki.K
```

> ※ フォルダを作り、Dockerfileは開発用途にわけて更新します。
