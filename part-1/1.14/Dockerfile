FROM ruby:2.6.0
WORKDIR /app
RUN apt-get update -qq && apt-get install -y build-essential nodejs
COPY Gemfile* ./
RUN gem install bundler && bundle install
COPY . .
RUN rails db:migrate
EXPOSE 3000
CMD [ "rails", "s" ]
