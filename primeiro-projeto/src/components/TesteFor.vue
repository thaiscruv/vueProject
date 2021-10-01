<template>
  <div class="teste-for">
    <h2>Teste For</h2>
    <ul>
      <li v-for="animal of animais" :key="animal.id">
        <img :src="animal.url" :alt="animal.nome" />
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "TesteFor",
  data() {
    return {
      animais: [
        {
          id: 1,
          nome: "Gatineo",
          url:
            "https://www.petz.com.br/blog/wp-content/uploads/2019/07/vida-de-gato.jpg",
        },
        {
          id: 2,
          nome: "Doguineo",
          url:
            "https://www.petz.com.br/blog/wp-content/uploads/2021/03/piercing-para-cachorro-2.jpg",
        },
      ],
    };
  },
};
</script>

<style scoped></style>
