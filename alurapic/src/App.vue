<template>
  <div>
    <h1>{{ titulo }}</h1>
    <ul>
      <li v-for="foto of fotos" :key="foto">
        <img :src="foto.url" :alt="foto.titulo" />
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      titulo: "Alurapic",
      fotos: [
        {
          url: "https://img.freepik.com/fotos-gratis/lindo-retrato-de-cachorro_23-2149218451.jpg?w=1380&t=st=1660149698~exp=1660150298~hmac=b04684fef3e956df64c429d26cbb1704efc66f4344353797bd9800332ebf1057",
          titulo: "cachorro",
        },
        {
          url: "https://img.freepik.com/fotos-gratis/lindo-retrato-de-cachorro_23-2149218451.jpg?w=1380&t=st=1660149698~exp=1660150298~hmac=b04684fef3e956df64c429d26cbb1704efc66f4344353797bd9800332ebf1057",
          titulo: "cachorro2",
        },
      ],
    };
  },
};
</script>

<style>
</style>
