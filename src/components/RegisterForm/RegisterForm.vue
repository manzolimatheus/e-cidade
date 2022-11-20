<template>
  <form>
    <header>
      <img src="/img/Logo.png" alt="Logo e-cidade" width="200" />
      <p class="text-secondary">Seu portal do cidadão</p>
    </header>

    <div class="form-group">
      <label for="name">Nome Completo</label>
      <input type="text" id="name" v-model="name" placeholder="Nome Completo" />
    </div>

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
      <router-link to="/login">Já tem uma conta? Entrar</router-link>
      <br /><br />
      <button type="submit" class="button-safe p-4">Cadastrar</button>
    </div>
  </form>
</template>

<script>
export default {
  data() {
    return {
      email: "",
      password: "",
      name: "",
    };
  },
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
