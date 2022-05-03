# Pages and routing 
## Sometimes you might need to create dynamic routes or nested routes or you might need to further configure the router property. This chapter will go through everything you need to know in order to get the best out of your router.
---
# How does Routing works on nuxt ?
## Nuxt automatically generates the vue-router configuration based on your file tree of Vue files inside the pages directory. When you create a .vue file in your pages directory you will have basic routing working with no extra configuration needed.
<br>

# Buut, HOW DOES IT WORKS ?
## If we look in ".nuxt" folder (that you are suposed to not change, this is for didatical purpose), You´ll see that as i create .vue files in the pages folder, the routing file is writen/changed.

````
*Folder structure
pages/
--| user/
-----| index.vue
-----| one.vue
--| index.vue

*./nuxt/router/index.js
router: {
  routes: [
    {
      name: 'index',
      path: '/',
      component: 'pages/index.vue'
    },
    {
      name: 'user',
      path: '/user',
      component: 'pages/user/index.vue'
    },
    {
      name: 'user-one',
      path: '/user/one',
      component: 'pages/user/one.vue'
    }
  ]
}
````

# How about links, Wont we use more routerLink ?
## We still using routerLink for redirect the user to other pages, and We still allowed to use the vueRouterlink, but We recommend to use NuxtLink that load your js files when the page is loaded before the user clicks in the button.

<br>

````
<div class="container mx-auto">
    <NuxtLink :to="{ name:'a-empresa' }">
</div>
````

