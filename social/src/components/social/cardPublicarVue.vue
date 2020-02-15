<template>
    <div class="row">
        <grid-vue class="input-field" tamanho="12">
          <textarea v-model="pensamento" class="materialize-textarea"></textarea>
          <label>O que você esta pensando? </label>
        </grid-vue>
        <p>
            <grid-vue v-if="pensamento" class="btn waves-effect waves-light col s" tamanho="2 offset-s10">
            Publicar
            </grid-vue>
        </p>
    </div>
</template>

<script>
import gridVue from '@/components/layouts/grids/gridVue';
export default {
  name: 'cardPublicarvue',
  props: [],
  data () {
    return {
        pensamento : ''
    }
  },
  components :{
     gridVue
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
