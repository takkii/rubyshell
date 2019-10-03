### rubyshell

*dockerのコンテナ、rubyshellを詰め込んだ*

技術的な環境構築のための実験的コンテナ。

とりあえず試すときに使う環境

使い方

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

> MITライセンスです

> 作成者 Takauki.K
