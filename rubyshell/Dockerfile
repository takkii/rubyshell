# distro os.
FROM ubuntu:18.04
# mkdir users
LABEL maintainer="Takayuki.K <karuma.reasonp@gmail.com>"
# RUN: docker build
RUN echo "now building..."
# CMD: docker run
CMD echo "now running..."
# build package
RUN apt-get update && apt-get install -y git rbenv ruby-build ruby-dev  && apt-get clean
RUN git clone https://github.com/rbenv/ruby-build.git "$(rbenv root)"/plugins/ruby-build

RUN rbenv install -l
RUN rbenv install 2.6.5

RUN rbenv init -
RUN echo 'eval "$(rbenv init -)"' >> ~/.bashrc
RUN echo 'export RUBYOPT="--jit"' >> ~/.bashrc
RUN rbenv global 2.6.5

# install
RUN rbenv exec gem install bundler rails && gem cleanup all

# All Docker remove command. Clean up all. 
# docker system prune 