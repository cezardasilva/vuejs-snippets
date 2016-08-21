# vuejs-snippets

[![apm](https://img.shields.io/apm/dm/vuejs-snippets.svg)](https://atom.io/packages/vuejs-snippets)
[![apm](https://img.shields.io/apm/l/vuejs-snippets.svg?maxAge=2592000)](https://atom.io/packages/vuejs-snippets)
[![apm](https://img.shields.io/apm/v/vuejs-snippets.svg?maxAge=2592000)](https://atom.io/packages/vuejs-snippets)

VueJS Components Snippets for Atom

---

## Types

- .text.html.vue

## Snippets

### Vue Component

prefix: component

body:
  ```
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

### Vue Validator

  prefix: validator

  body:
    ```
    Vue.validator("validatorName", function (val) {
      return true
    });
    ```

### Vue Validator Local

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

### Vue Router map

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
