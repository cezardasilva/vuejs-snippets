# Vue.js Snippets [![apm](https://img.shields.io/apm/dm/vuejs-snippets.svg)](https://atom.io/packages/vuejs-snippets) [![apm](https://img.shields.io/apm/l/vuejs-snippets.svg?)](https://atom.io/packages/vuejs-snippets) [![apm](https://img.shields.io/apm/v/vuejs-snippets.svg?)](https://atom.io/packages/vuejs-snippets)

Vue.js Snippets for Atom

## Types
- .text.html.vue
- .text.js

## Snippets

### Vue Component
prefix: template
body:
  ```Vue
  <template>
    <div id='YourComponentName'>
      <!--You component contents goes here-->
    </div>
  </template>
  <script>
    export default {
      name: "YourComponentName",
      data(){
        return {
          //Component Data
          example: true,
          foo: "bar"
        }
      },

      created(){
        //On Component created
      },

      methods: {
        functionExample(){
          //Basic Component method
        }
      }
    }
  </script>
  ```

## Vue Router

### Router
  prefix: router
  body:
  ```javascript
  import Vue from 'vue'
  import VueRouter from 'vue-router'

  Vue.use(VueRouter)

  const routes = [
    {
      name: "YourRouteName",
      path: "/",
      component: YourComponent
    }
  ]

  export const router = new VueRouter({
    routes: routes,
    scrollBehavior (to, from, savedPosition) {
      return { x: 0, y: 0 }
    }
  })
  ```

## Vue filter

### New Filter
  prefix: filter
  body:
  ```javascript
  Vue.filter('yourfiltername', (value) => {
    return true
  })
  ```
## Vue Resource

### Get

  prefix: get

  body:

  ```javascript
  this.$http.get(URL).then((result) => {

	}, (error) => {

	})
  })
  ```

### Post

  prefix: post

  body:

  ```javascript
  this.$http.post(URL, PARAMS).then((response) => {

	}, (error) => {

	})
  ```

### Put

  prefix: put

  body:

  ```javascript
  this.$http.put(URL, PARAMS).then((response) => {

	}, (error) => {

	})
  ```

### Delete

  prefix: delete

  body:

  ```javascript
  this.$http.delete(URL, PARAMS).then((response) => {

	}, (error) => {

	})
  ```
