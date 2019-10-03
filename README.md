### rubyshell

*dockerのコンテナ、rubyshellを詰め込んだ*

技術的な環境構築のための実験的コンテナ。

とりあえず試すときに使う環境

使い方 ( rubyshellの部分は、ビルド名で任意です )

```ruby
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
```

環境

```markdown
ruby 2.6.5 (+JIT)

rails 6.0.0
```

> MITライセンスです

> 作成者 Takauki.K
