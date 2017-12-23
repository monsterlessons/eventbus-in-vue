<template>
  <div>
    <h3>{{upperCasedName()}}</h3>
    <div>
      {{description}}
    </div>
    <div>
      {{isActive}}
    </div>
  </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      default: 'Not set'
    },
    description: String,
    isActive: Boolean
  },
  methods: {
    upperCasedName () {
      return this.name.toUpperCase()
    }
  }
}
</script>
