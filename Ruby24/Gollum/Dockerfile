FROM       altran/ruby-2.4
MAINTAINER Jinmin Hu <jinmin.hu@altran.com>

RUN apt-get -y update && apt-get -y install libicu-dev
RUN gem install gollum
RUN gem install redcarpet org-ruby
VOLUME /wiki
WORKDIR /wiki
CMD ["gollum", "--port", "80"]
EXPOSE 80

