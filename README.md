### A docker container for verification 

_※ build (rubyshell-ubuntu 18.04 / hakoirimusume-ubuntu 20.4.1)_

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
docker build -t personal .

# run
docker run -it rubyshell /bin/bash
docker run -it hakoirimusume /bin/bash
docker run -it personal /bin/bash

# exec
docker exec -it rubyshell /bin/bash --login
docker exec -it hakoirimusume /bin/bash --login
docker exec -it personal /bin/bash --login
```

### docker container

```markdown
docker pull takkii/dockerhub:personal
```

[takkii/dockerhub](https://hub.docker.com/r/takkii/dockerhub)

### Env

```markdown

Windows10, powershell and WSL and WSL2 → ○ build success
MacOS Catalina → ○ build success

※ rubyshell is MIT License.
```
