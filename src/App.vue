<template>
  <div>
    <h1>Hello Vue!</h1>
    <loginForm/>
    <successMessage/>
  </div>
</template>

<script>
import loginForm from './LoginForm.vue'
import successMessage from './SuccessMessage.vue'
export default {
  components: {
    loginForm,
    successMessage
  }
}
</script>
