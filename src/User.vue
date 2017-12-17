<template>
  <div>
    <h3>{{name}}</h3>
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
  props: ['name', 'description', 'isActive']
}
</script>
