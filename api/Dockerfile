FROM ruby:2.5.5
RUN apt-get update -qq && apt-get install -y build-essential libpq-dev nodejs

RUN mkdir -p /api
RUN cd /api

COPY . .

COPY Gemfile /api/Gemfile
COPY Gemfile.lock /api/Gemfile.lock

RUN gem install bundler
RUN bundle install

EXPOSE 3000
CMD ["bundle", "exec", "puma", "-C", "config/puma.rb"]
