<template>
  <div class="container-bg">
    <ContainerBlock>
      <RegisterForm/>
    </ContainerBlock>
  </div>
</template>

<script>
import ContainerBlock from "@/components/ContainerBlock/ContainerBlock.vue";
import RegisterForm from "@/components/RegisterForm/RegisterForm.vue";

export default {
  components: { RegisterForm, ContainerBlock },
};
</script>

<style scoped>
.container-bg {
  background: linear-gradient(
      to bottom,
      rgba(0, 0, 0, 0.2) 0%,
      rgb(231, 231, 231) 60%
    ),
    url("https://media.tenor.com/f3Yzj3OxyX0AAAAd/people-crowd.gif");
  background-attachment: fixed;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.container {
  width: 25%;
  /* height: 40%; */
}

@media (max-width: 768px) {
  .container {
    width: 90%;
  }
}
</style>
