FROM       ubuntu:14.04
MAINTAINER Jinmin Hu <jinmin.hu@altran.com>

RUN apt-get update && apt-get install --yes build-essential automake git
RUN apt-get update && apt-get install --yes wget
RUN wget --no-check-certificate https://ftp.ruby-lang.org/pub/ruby/2.4/ruby-2.4.0-preview1.tar.gz
RUN tar xzvf ruby-2.1.3.tar.gz
RUN cd ruby-2.4.0-preview1 && ./configure --disable-install-doc
RUN cd ruby-2.4.0-preview1 && make
RUN cd ruby-2.4.0-preview1 && make install
RUN ln -s /usr/local/bin/ruby /usr/bin/ruby
