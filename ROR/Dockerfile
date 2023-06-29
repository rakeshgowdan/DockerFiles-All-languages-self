FROM ruby:3.1.2
WORKDIR /app
COPY Gemfile Gemfile.lock ./
RUN bundle install
COPY . .
EXPOSE 3000
ENTRYPOINT ["dotenv", "-f", ".env.staging", "bundle", "exec", "rails", "s", "-p", "3000", "-b", "0.0.0.0"]