# distro os.
FROM ubuntu:focal

# mkdir users
LABEL maintainer="Takayuki Kamiyama <karuma.reason@gmail.com>"

# tzdata/Tokyo
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get install -y tzdata
# timezone setting
ENV TZ=Asia/Tokyo 

# build package
RUN apt-get update && apt-get install -y \ 
git rbenv ruby-build ruby-dev sqlite3 libxslt1-dev libxml2-dev build-essential patch \
libsqlite3-dev libcurl4-openssl-dev curl nodejs libmagickcore-dev libmagickwand-dev && apt-get clean

# rbenv
RUN git clone https://github.com/rbenv/ruby-build.git "$(rbenv root)"/plugins/ruby-build

RUN rbenv install -l
RUN rbenv install 2.7.1

RUN rbenv init -
RUN echo 'eval "$(rbenv init -)"' >> ~/.bashrc
RUN echo 'export RUBYOPT="--jit"' >> ~/.bashrc
RUN rbenv global 2.7.1

# install
RUN rbenv exec gem install bundler rails rmagick sqlite3 zinbei zinbeijett himekuri tanraku && gem cleanup all

# All Docker remove command. Clean up all.
# docker system prune


