<template>
  <span>
    <header>
       <navbar-vue cor="green darken-4" logo="VueJs">
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/login">Entrar</router-link></li>
        <li><router-link to="/cadastro">Cadastre-se</router-link></li>
       </navbar-vue>
    </header>
    <main class="container">
      <div class="row">
        <grid-vue tamanho="4">
          <card-vue>
           <slot name="menuesquerdo" />
          </card-vue>
        </grid-vue>
        <grid-vue tamanho="8">
           <slot name="conteudo" />
        </grid-vue>
      </div>
    </main>
    <footer-vue cor="green darken-4" logo="VueJs" descricao="Aplicação utilizando
    o vueJS" ano="2020" >
        <li><router-link class="grey-text text-lighten-3" to="/">Home</router-link></li>
        <li><router-link class="grey-text text-lighten-3" to="/login">Entrar</router-link></li>
        <li><router-link class="grey-text text-lighten-3" to="/cadastro">Cadastre-se</router-link></li>
    </footer-vue>
    
  </span>
</template>

<script>
import navbarVue from '@/components/layouts/menus/headerVue';
import footerVue from '@/components/layouts/rodape/footerVue';
import gridVue from '@/components/layouts/grids/gridVue';
import cardVue from '@/components/layouts/cards/cardVue';

export default {
  name: 'Site',
  components :{
     navbarVue,
     gridVue,
     cardVue,
     footerVue
  }
}
</script>

<style>
</style>
