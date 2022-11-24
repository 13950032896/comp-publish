<template>
  <div>
    <button @click="click">
      <slot></slot>
    </button>
  </div>
</template>

<script>
export default {
  name: 'LgButton',
  inheritAttrs: false,
  methods: {
    click(evt) {
      this.$emit('click', evt)
      evt.preventDefault()
    }
  }
}
</script>

<style>

</style>
