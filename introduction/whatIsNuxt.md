# What is nuxt ?
## It´s a framework to build vue.js apps
# So, Nuxt is vue ?
## YEP!!
<br>



# But why do we need a framework for a framwework ?

## Nuxt. js enables developers to build Server Side Rendered applications in which a Node. js server will deliver HTML to the client based on your Vue components (rather than running JavaScript on the client side). This will allow for better SEO than traditional SPAs built using Vue.
<br>

<div align="center">

# Nuxt, is a powerfull vue.js

![](https://nuxt-community.github.io/awesome-nuxt/media/awesome-nuxt-logo.svg)



## With dinamic routing and optmization for SEO.

# Getting through those powers that came with Nuxt
- ## Server side rendering
- ## Code splitting
- ## Starter template (as vue)
- ## Great folder structurs by default
- ## Easy ES6/ES7 Compilation
- ## A lot of modules (auth, google api, social login)
----
- ## Dinamic routing
- ## Data fetching
- ## Meta tags (SEO)
- ## Progress bar
- ## Middleware
- ## Plugins
- ## Layout
</div>
<br>

# How to install nuxt
- ## Getting started 

````
// yarn
yarn create nuxt-app <project-name>

//npm
npx create nuxt-app <project-name>

// it will ask some questions
- js or ts
- yarn or npm
- UI framework
- Nuxt modules
- Linting tools 
- test framework
- rendering mode
- development tools
- tracker systems (git/gitlab)
-----------------------

cd <project-name>
yarn dev / yarn run dev // it will run in the port 3000

````
<br>

# Folder Structure

## You can create the following extra directories, some of which have special behaviors. Only `pages` is required; you can delete them if you don't want to use their functionality.

<br>

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


