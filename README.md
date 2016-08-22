# vuejs-snippets

[![apm](https://img.shields.io/apm/dm/vuejs-snippets.svg)](https://atom.io/packages/vuejs-snippets)
[![apm](https://img.shields.io/apm/l/vuejs-snippets.svg?maxAge=2592000)](https://atom.io/packages/vuejs-snippets)
[![apm](https://img.shields.io/apm/v/vuejs-snippets.svg?maxAge=2592000)](https://atom.io/packages/vuejs-snippets)

VueJS Snippets for Atom

---

## Types

- .text.html.vue
- .text.js


## Snippets


### Vue Component

prefix: component

body:
  ```Vue
  <template>
    //You component contents goes here, only html.
  </template>

  <script>

  export default {
    name: "ComponentName",
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

## Vue Validator

### Global
  prefix: validator

  body:
  ```
  Vue.validator("validatorName", function (val) {
    return true
  });
  ```

### Local

  prefix: validators

  body:

  ```
  [..]
  validators: {
    nameOfValidator: function (val) {
      return true
    }
  },
  [...]
  ```  

## Vue Router

### Map

  prefix: map

  body:

  ```  
  router.map({
    '/example': {
      component: Example,
      subRoutes:{
        '/subrouter': {
          component: SubRouter
        }
      }
    }
  })
  ```

## Vue Resource

### Get

  prefix: get

  body:

  ```  
  CONTEXT.$http.get(URL).then((result) => {

		}, (error) => {

		})
  })
  ```

### Post

  prefix: post

  body:

  ```
  CONTEXT.$http.post(URL, PARAMS).then((response) => {

	}, (error) => {

	})
  ```

### Put

  prefix: put

  body:

  ```
  CONTEXT.$http.put(URL, PARAMS).then((response) => {

	}, (error) => {

	})
  ```

### Delete

  prefix: delete

  body:

  ```
  CONTEXT.$http.delete(URL, PARAMS).then((response) => {

	}, (error) => {

	})
  ```
