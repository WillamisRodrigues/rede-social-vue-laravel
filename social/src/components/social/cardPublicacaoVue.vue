<template>
  <span>
        <div v-if="img" class="card-image">
            <img v-bind:src="img">
            <span class="card-title">{{titulo || ''}}</span>
        </div>
        <div v-if="descricao" class="card-content">
            <p>
                {{descricao}}
            </p>
       </div>
  </span>
</template>

<script>

export default {
  name: 'cardPublicacaovue',
  props: ['img','titulo','descricao'],
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
