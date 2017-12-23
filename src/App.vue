<template>
  <div>
    <h1>Hello Vue!</h1>
    <my-user
      v-for='user in users'
      :name='user.name'
      :description='user.description'
      :is-active='user.isActive'
      :key='user.name'
    />
    <my-user />
  </div>
</template>

<script>
import user from './User.vue'

export default {
  data () {
    return {
      users: [
        {name: 'Alex', description: 'This is admin', isActive: true},
        {name: 'Jack', description: 'This is manager', isActive: false},
        {name: 'John', description: 'This is client', isActive: false}
      ]
    }
  },
  components: {
    myUser: user
  }
}
</script>
