<template>
  <login-template>
    <span slot="menuesquerdo">
      <img src="https://lh3.googleusercontent.com/proxy/ahYmmQg8J7JCnZxqrjYzW8ituJWt3dwTPTIGZSv1YU30E0vPgr33RsIRI2KXumceQuDLjGoNPlZiIhRQLknIjWfx-tQb5Mx7M2IQjYrj9E7mEmWPVrugGWDiiwYRN52zEVAb3UIZ6-E9UN16B-qy5_-L7QulyeM8uvv4NJuqykiexid-hWyx16LML9cZjwDly5j65GgHlXjbAECmkw" class="responsive-img" alt="">
    </span>
    <span slot="principal">
         <h2>Login</h2>
        <input type="text" placeholder="E-mail" value="">
        <input type="text" placeholder="Senha" value="">
        <button class="btn"> Entrar </button>
        <router-link class="btn orange" to="/cadastro"> Cadastre-se </router-link>
      </span>
  </login-template>
</template>

<script>
import LoginTemplate from '@/templates/LoginTemplate';

export default {
  name: 'Login',
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
