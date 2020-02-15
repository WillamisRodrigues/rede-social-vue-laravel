<template>
  <login-template>
    <span slot="menuesquerdo">
      <img src="https://lh3.googleusercontent.com/proxy/ahYmmQg8J7JCnZxqrjYzW8ituJWt3dwTPTIGZSv1YU30E0vPgr33RsIRI2KXumceQuDLjGoNPlZiIhRQLknIjWfx-tQb5Mx7M2IQjYrj9E7mEmWPVrugGWDiiwYRN52zEVAb3UIZ6-E9UN16B-qy5_-L7QulyeM8uvv4NJuqykiexid-hWyx16LML9cZjwDly5j65GgHlXjbAECmkw" class="responsive-img" alt="">
    </span>
    <span slot="principal">
         <h2>Cadastro</h2>
        <input type="text" placeholder="Nome" value="">
        <input type="email" placeholder="E-mail" value="">
        <input type="password" placeholder="Senha" value="">
        <input type="password" placeholder="Confirmar Senha" value="">
        <button class="btn"> Enviar </button>
        <router-link class="btn orange" to="/login"> Já possue conta? </router-link>
    </span>
    
  </login-template>
</template>

<script>
import LoginTemplate from '@/templates/LoginTemplate';

export default {
  name: 'Cadastro',
  data () {
    return {
    }
  },
  components :{
    LoginTemplate
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
