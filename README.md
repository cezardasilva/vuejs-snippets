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

### Vue Modal Component

  prefix: modal

  body:

    <template>
      <modal :show.sync="showModal">
        <h2 slot="header">{{$t("change_password.title")}}</h2>
        <div slot="body">
          //You component contents goes here, only html.
        </div>
        <div slot="footer" class="text-center">
        </div>
      </modal>
    </template>

    <script>
    import Modal from './interface/Modal.vue'

    export default {
      name: "ComponentName",
      components: { Modal },
      data(){
        return {
          //Component Data
          showModal: false,
        }
      },

      created(){
        //On Component created
        this.showModal = true;
      },

      methods: {
        functionExample(){
          //Basic Component method
        }
      }
    }
    </script>
