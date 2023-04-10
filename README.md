# This repository is about the first one question of the WS Work Front-end Test

### The topics below are about the project itself, whose question asked to choose between Next.js (React) or Nuxt.js (Vue), I chose to develop this application with Nuxt.js and with the yarn package manager because it is faster in project creation.

>Please read until the end, I will show you the final result.

## Build Setup

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out the [documentation](https://nuxtjs.org).

## Special Directories

You can create the following extra directories, some of which have special behaviors. Only `pages` is required; you can delete them if you don't want to use their functionality.

### `assets`

The assets directory contains your uncompiled assets such as Stylus or Sass files, images, or fonts.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/assets).

### `components`

The components directory contains your Vue.js components. Components make up the different parts of your page and can be reused and imported into your pages, layouts and even other components.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/components).

### `layouts`

Layouts are a great help when you want to change the look and feel of your Nuxt app, whether you want to include a sidebar or have distinct layouts for mobile and desktop.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/layouts).

### `pages`

This directory contains your application views and routes. Nuxt will read all the `*.vue` files inside this directory and setup Vue Router automatically.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/get-started/routing).

### `plugins`

The plugins directory contains JavaScript plugins that you want to run before instantiating the root Vue.js Application. This is the place to add Vue plugins and to inject functions or constants. Every time you need to use `Vue.use()`, you should create a file in `plugins/` and add its path to plugins in `nuxt.config.js`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/plugins).

### `static`

This directory contains your static files. Each file inside this directory is mapped to `/`.

Example: `/static/robots.txt` is mapped as `/robots.txt`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/static).

### `store`

This directory contains your Vuex store files. Creating a file in this directory automatically activates Vuex.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/store).
## The requested layout was:
![image](https://user-images.githubusercontent.com/106850969/230840646-9b91e44b-1ca4-43a1-85e9-ba74f2509cc2.png)
## Tech Recruiter said I was free to develop the app any way I wanted, so I respected the layout and styled the rest, I made a component-based application and created an image carousel with the middle content.
![image](https://user-images.githubusercontent.com/106850969/230841312-444f032a-4739-45d4-a4d4-b8738cdd6f92.png)
![image](https://user-images.githubusercontent.com/106850969/230841029-cbf3f1dd-088f-4849-a2c9-6ad90f7db54b.png)
## Check out the special effects! (Take a Look at the carousel)
![Questao 1 - WS Work Front end test](https://user-images.githubusercontent.com/106850969/230841519-56fcc227-5757-415c-a069-41ef8355710b.gif)

> If you are curious, the Carousel was implemented in components/CarouselComponent.vue
