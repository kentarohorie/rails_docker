## Development Setup
```bash
docker run -v $PWD:/app -it --rm ruby:2.6.4 bash

cd /app

bundle init

# Uncomment this line.
# # gem 'rails'

bundle install -j `nproc`

rails new .

docker-compose build

# and setup rails, db:create and more.
```

nginx config is for using puma socket.
