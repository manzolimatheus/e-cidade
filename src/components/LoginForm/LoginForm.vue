<template>
  <form>
    <header>
      <img src="/img/Logo.png" alt="Logo e-cidade" width="200" />
      <p class="text-secondary">Seu portal do cidadão</p>
    </header>

    <div class="form-group">
      <label for="email">E-mail</label>
      <input type="email" id="email" v-model="email" placeholder="E-mail" />
    </div>

    <div class="form-group">
      <label for="password">Senha</label>
      <input
        type="password"
        id="password"
        v-model="password"
        placeholder="Senha"
      />
    </div>
    <div class="text-center">
      <router-link to="/register">Não tem uma conta? Cadastre-se</router-link>
      <br /><br />
      <button type="submit" class="button-safe p-4">Entrar</button>
    </div>
  </form>
  <p class="my-4">OU</p>
  <AuthButtons />
</template>

<script>
import AuthButtons from "./AuthButtons.vue";

export default {
  data() {
    return {
      email: "",
      password: "",
    };
  },
  components: { AuthButtons },
};
</script>

<style scoped>
form {
  display: flex;
  flex-direction: column;
  gap: 20px;
  width: 100%;
}

header {
  text-align: center;
}
</style>
