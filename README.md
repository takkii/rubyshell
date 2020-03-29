# rubyshell

【 技術的な環境構築のための実験的コンテナ 】

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](LICENSE)![GitHub release](https://img.shields.io/github/release/takkii/rubyshell.svg?style=flat)[![GitHub Status](https://img.shields.io/github/last-commit/takkii/rubyshell.svg?style=flat)](GitHub)

[ 起動例 ]

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

### コンテナのバージョン毎に構成するRubyなどが違います。

[ 動作確認 & ライセンス & 作成者 ]

```markdown

Windows 10 ( powershell & WSL ) → ○
MacOS Catalina → ○

Windows 10 Insider Program → ⚠
→ Dockefile内6行目付近のシステムアップデートで、
  エラーになりビルド停止することがあります。

※ rubyshellはMITライセンスです

作成者 Takauki Kamiyama
```
