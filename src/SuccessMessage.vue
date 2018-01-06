<template>
  <h3 v-if='email'>Thanks for loggining, {{email}}</h3>
</template>

<script>
  export default {
    props: ['email']
  }
</script>
