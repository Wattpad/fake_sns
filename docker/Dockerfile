FROM ruby
MAINTAINER Logan Attwood <logan@jnickel.com>

RUN gem install specific_install
RUN gem specific_install https://github.com/Wattpad/fake_sns.git

EXPOSE 9292
ENV RACK_ENV=production

ENTRYPOINT ["/usr/local/bundle/bin/fake_sns"]
