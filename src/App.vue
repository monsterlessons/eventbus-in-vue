<template>
  <div>
    <h1>Hello Vue!</h1>
    <loginForm :onLogin='onLogin' />
  </div>
</template>

<script>
import loginForm from './LoginForm.vue'
export default {
  data () {
    return {
    }
  },
  components: {
    loginForm
  },
  methods: {
    onLogin (data) {
      console.log('child component said login', data)
    }
  }
}
</script>
