<template>
  <h3 v-if='email'>Thanks for loggining, {{email}}</h3>
</template>

<script>
  import {eventBus} from './main'
  export default {
    data () {
      return {
        email: ''
      }
    },
    created () {
      eventBus.$on('login', data => {
        this.email = data.email
      })
    }
  }
</script>
