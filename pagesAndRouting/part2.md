# Pages and routing
## As we already saw, when I create a .vue file in the pages folder it became automatically a route, the same is for folders.

## The same example of the last topic :
````
pages/                    
--| user/
-----| index.vue    => https://localhost/user/ 
-----| one.vue      => https://localhost/user/one 
--| index.vue => https://localhost/
````

- ### Naming your files with "index.vue" it will be set as the main page for the folder
    * ### For example you are building a ecommerce and want to set a main page for t shirts, that will be like:
    ````
    pages/  
    --| shirts/
    -----| index.vue 
    -----| types.vue 
    ````
    ## So here the URL will be "localhost/shirts/", not shirts/index.vue <br> The Index is the main file and the name is set as the folder´s name in the URL.

# Dynamic routes
### Dynamic pages can be created when you don't know the name of the page due to it coming from an API or you don't want to have to create the same page over and over again. To create a dynamic page you need to add an underscore before the .vue file name or before the name of the directory, if you want the directory to be dynamic. You can name the file or directory anything you want but you must prefix it with an underscore.

### If you've defined a file named _slug.vue in your pages folder, you can access the value using the context with params.slug

````
<template>
  <h1>{{ slug }}</h1> //same as: {{ $route.params }}
</template>

<script>
  export default {
    async asyncData({ params }) {
      const slug = params.slug // When calling /abc the slug will be "abc"
      return { slug }
    }
  }
</script>
````
 ### ex 2
 ````
 <template>
  <h1>{{ book }} / {{ slug }}</h1>
</template>

<script>
  export default {
    async asyncData({ params }) {
      const book = params.book
      const slug = params.slug
      return { book, slug }
    }
  }
</script>
