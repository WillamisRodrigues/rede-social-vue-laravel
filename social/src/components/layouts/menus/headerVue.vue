<template>
  <nav v-bind:class='cor'>
    <div class="nav-wrapper container">
      <router-link class="brand-logo" v-bind:to="url || '/'">{{logo || 'Site' }}</router-link>
      <ul id="nav-mobile" class="right hide-on-med-and-down">
        <slot />
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'navbarVue',
  props: ['logo','url','cor'],
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
