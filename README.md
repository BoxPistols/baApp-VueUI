# ba-app

> A Vue.js project

## Tree

├── README.md
├── build
├── config
├── dist
├── index.html
├── node_modules
├── package.json
├── src
│   ├── App.vue
│   ├── assets
│   ├── components
│   │   ├── MyCanvas.vue
│   │   ├── page1.vue
│   │   └── page2.vue
│   ├── main.js
│   └── router
│       └── index.js
├── static
└── yarn.lock


## Build Setup

``` bash
# install dependencies
yarn install


### if not install

  # add pug
  yarn add pug --dev
  yarn add -D pug pug-loader

  # add sass
  yarn add sass-loader node-sass


# serve with hot reload at localhost:8080
yarn run dev

# build for production with minification
yarn run build

# build for production and view the bundle analyzer report
yarn run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
