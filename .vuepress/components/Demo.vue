<template lang="html">
  <div class="app-demo">
    <p>{{ content }}</p>

    <div>
      <button type="button" @click="onAwesome">Awesome!</button>
      <button type="button" @click="onLame">Lame...</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Demo',
  data: function() {
    return {
      content: 'How about this Vue Demo Component?'
    }
  },
  methods: {
    onAwesome: function() {
      alert('Cool!')
    },
    onLame: function() {
      alert('Yep... pretty lame actually')
    }
  }
}
</script>

<style lang="scss" scoped>
  .app-demo {
    border: 1px solid black;
  }
</style>
