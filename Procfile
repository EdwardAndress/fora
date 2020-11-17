worker: bundle install
worker: bundle exec rails webpacker:install
worker: bundle exec rails webpacker:compile
worker: bin/rails db:migrate
web: bundle exec puma -t 5:5 -p ${PORT:-3000} -e ${RACK_ENV:-production}