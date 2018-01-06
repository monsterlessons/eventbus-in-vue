<template>
  <div>
    <h1>Hello Vue!</h1>
    <loginForm :onLogin='onLogin' />
    <successMessage :email='email' />
  </div>
</template>

<script>
import loginForm from './LoginForm.vue'
import successMessage from './SuccessMessage.vue'
export default {
  data () {
    return {
      email: ''
    }
  },
  components: {
    loginForm,
    successMessage
  },
  methods: {
    onLogin (data) {
      this.email = data.email
    }
  }
}
</script>
