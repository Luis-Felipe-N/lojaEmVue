<script setup>
import { ref } from 'vue'

const produtos = ref([
  {
    nome: 'Caneca massa',
    preco: 19,
    imagem: 'mug01.png'
  },
    {
    nome: 'Caneca muito massa',
    preco: 19,
    imagem: 'mug02.png'
  },
    {
    nome: 'Caneca muito muito massa',
    preco: 19,
    imagem: 'mug03.png'
  }
])

function handleInput(e) {
  text.value = e.target.value
}
</script>

<template>
<div class="container">
  <div v-for="produto in produtos">
    <div>
      <img :src="require(`@/assets/${produto.imagem}.png`)" alt="">
      <strong>{{ produto.nome }}</strong>
      <span>R$ {{ produto.preco }}</span>
    </div>
  </div>
</div>
</template>

<style scoped>
.container {
  display: flex;
  padding: 0 5%;
}

.container div {
  display: flex;
  flex-direction: column;
}

.container div strong {
  font-size: 1.2rem;
}

</style>
