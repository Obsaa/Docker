FROM ruby

RUN apt-get update -qq && apt-get install -y build-essential --no-install-recommends apt-utils
EXPOSE 3000
ONBUILD COPY . /opt/app
ONBUILD WORKDIR /opt/app
ONBUILD RUN gem install bundler rubygems-bundler
ONBUILD RUN gem install rails
