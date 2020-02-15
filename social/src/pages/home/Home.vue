<template>
  <site-template>
    <span slot="menuesquerdo">
            <div class="row valign-wrapper">
              <grid-vue tamanho="4">
                <img src="https://materializecss.com/images/yuna.jpg" alt="" class="circle responsive-img"> <!-- notice the "circle" class -->
              </grid-vue>
              <grid-vue tamanho="8">
                <span class="black-text">
                  <h5>Maria Silva</h5>
                  Add the "circle" class to it to make it appear circular.
                </span>
              </grid-vue>
            </div>
    </span>
    <span slot="conteudo">
        <card-publicar-vue/>
        <card-conteudo-vue 
        perfil="https://materializecss.com/images/yuna.jpg"
        nome="Maria Silva" 
        data="13/02/2020 01h51">
        
        <card-publicacao-vue 
        img="https://materializecss.com/images/sample-1.jpg" 
        titulo="Card Title" 
        descricao="I am a very simple card. I am good at containing small bits of information.
        I am convenient because I require little markup to use effectively." />
        </card-conteudo-vue>
    </span>
  
  </site-template>
</template>

<script>
 import siteTemplate from '@/templates/SiteTemplate';
 import cardConteudoVue from '@/components/social/cardConteudoVue';
 import cardPublicacaoVue from '@/components/social/cardPublicacaoVue';
 import cardPublicarVue from '@/components/social/cardPublicarVue';
export default {
  name: 'Home',
  data () {
    return {
    }
  },
  components :{
     siteTemplate,
     cardConteudoVue,
     cardPublicarVue,
     cardPublicacaoVue
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
