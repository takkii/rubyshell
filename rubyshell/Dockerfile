# distro os.
FROM ubuntu:bionic
# mkdir users
LABEL maintainer="Takayuki Kamiyama <karuma.reason@gmail.com>"
# build package
RUN apt update
RUN apt install git rbenv ruby-build ruby-dev sqlite3 libxslt1-dev libxml2-dev build-essential patch libsqlite3-dev libcurl4-openssl-dev curl nodejs libmagickcore-dev libmagickwand-dev
RUN apt autoremove

# rbenv
RUN git clone https://github.com/rbenv/ruby-build.git "$(rbenv root)"/plugins/ruby-build

RUN rbenv install -l
RUN rbenv install 2.7.0

RUN rbenv init -
RUN echo 'eval "$(rbenv init -)"' >> ~/.bashrc
RUN echo 'export RUBYOPT="--jit"' >> ~/.bashrc
RUN rbenv global 2.7.0

# install
RUN rbenv exec gem install bundler rails rmagick sqlite3 zinbei zinbeijett himekuri
# cleanup
RUN gem cleanup all

# All Docker remove command. Clean up all.
# docker system prune
