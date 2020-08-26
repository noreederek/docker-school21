FROM ruby:2.3.4

RUN apt-get update -yqq
RUN apt-get upgrade -y
RUN apt-get install -y sqlite3
RUN apt-get install -y gem
RUN gem install rails -v 4.1.8

#docker build -t ft-rails .
#docker build -t wrapper -f start.Dockerfile .
#docker run -it -p 3000:3000 wrapper

ONBUILD WORKDIR /opt/app
ONBUILD ADD ./sample_app/ /opt/app

ONBUILD EXPOSE 3000
ONBUILD RUN bundle install
