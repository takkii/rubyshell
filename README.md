### A docker container for verification ( rubyshell/hakoirimusume )

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](LICENSE)![GitHub release](https://img.shields.io/github/release/takkii/rubyshell.svg?style=flat)[![GitHub Status](https://img.shields.io/github/last-commit/takkii/rubyshell.svg?style=flat)](GitHub)

### how to use.

```markdown
# clone
git clone https://github.com/takkii/rubyshell.git

# directory
cd rubyshell/rubyshell
cd rubyshell/hakoirimusume

# build
docker build -t rubyshell .
docker build -t hakoirimusume .

# run
docker run -it rubyshell /bin/bash
docker run -it hakoirimusume /bin/bash
```

### docker container

_rubyshell or hakoirimusume change ubuntu version._

```markdown

Windows10, powershell and WSL and WSL2 → ○ build success
MacOS Catalina → ○ build success

※ rubyshell and hakoirimusume is MIT License.
```
