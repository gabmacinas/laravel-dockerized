# laravel-dockerized
1. modify servername in src/default.conf
2. cp env-example .env
3. modify .env to you needs
4. rm -rf src && rm -rf .git
5. laravel new src
6. docker compose up -d --build
  change hosts file to your needs


rm -rf ~/.docker/config.json | rm -rf .git && rm -rf src/ && cp env-example .env && laravel new src && dcup --build && dcmd composer require laravel/ui && dcmd artisan ui vue --auth && dcmd npm install && dcmd npm install vuetify vuetify-loader vue-router &&dcmd npm install vuex --save  && dcmd npm install sass sass-loader fibers deepmerge -D && dcrt && npmrunwatch


sed -i .bak 's/localhost/test.test/' nginx/default.conf

echo VAR2=`sed -n 's/VAR2=\(.*\)/\1/p' < txt'
