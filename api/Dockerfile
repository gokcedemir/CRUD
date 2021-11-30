FROM ruby:2.5.5

ADD . /api
WORKDIR /api
RUN apt-get update -qq && apt-get install -y nodejs postgresql-client
RUN gem install bundler
RUN bundle install

COPY entrypoint.sh /usr/bin/
RUN chmod +x /usr/bin/entrypoint.sh
ENTRYPOINT ["entrypoint.sh"]
EXPOSE 3000

CMD ["rails", "server", "-b", "0.0.0.0"]
