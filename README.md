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


[webpack.mix.js]
const mix = require('laravel-mix');

const VuetifyLoaderPlugin = require('vuetify-loader/lib/plugin');
const CaseSensitivePathsPlugin = require('case-sensitive-paths-webpack-plugin');

var webpackConfig = {
    plugins: [
        new VuetifyLoaderPlugin(),
        new CaseSensitivePathsPlugin()
    ]
}

mix.webpackConfig(webpackConfig);

mix.js('resources/js/app.js', 'public/js')
    .sass('resources/sass/app.scss', 'public/css');
[/webpack.mix.js]


[js/plugins/vuetify.js]
import Vue from 'vue'
import Vuetify from 'vuetify/lib'

Vue.use(Vuetify)

const opts = {}

export default new Vuetify(opts)
[/js/plugins/vuetify.js]

[app.js]
import Vuetify from 'your/vuetify/js/here';



under const app class add
vuetify: Vuetify,
[/app.js]

[modify mysql/default.conf files]
cp env-example .env
rm -rf .git 
rm -rf src/
laravel new src && dcup --build
dcmd composer require laravel/ui && dcmd artisan ui vue --auth
dcmd npm install 
dcmd npm run dev
dcmd npm install vuetify
dcmd npm install sass sass-loader fibers deepmerge -D
dcmd npm install vuetify-loader
dcmd npm install --save-dev case-sensitive-paths-webpack-plugin
npmrunwatch
