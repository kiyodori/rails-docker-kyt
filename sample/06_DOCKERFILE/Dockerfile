FROM ruby:2.7

WORKDIR /var/www

COPY ./src /var/www

RUN bundle config --local set path 'vendor/bundle' \
  && bundle install

CMD ["bundle", "exec", "ruby", "app.rb"]
