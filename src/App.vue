<template>
  <div>
    <h1>Hello Vue!</h1>
    <my-user />
  </div>
</template>

<script>
import user from './User.vue'

export default {
    components: {
      myUser: user
    }
}
</script>
