<template>
  <div v-bind:class="'col s'+ tamanho">
    <slot></slot>
   </div>
</template>

<script>
export default {
  name: 'gridvue',
  props: ['tamanho'],
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
