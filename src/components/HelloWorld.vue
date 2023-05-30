<script setup lang="ts">
defineProps<{
  name: string
  titulo: string
}>()
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ name }}</h1>
    <h2 class="name">{{ titulo }}</h2>
    <h3>
      Esta é a minha mensagem <br>
      <a href="https://alvdelci.github.io" target="_blank" rel="noopener">Link meu site</a>.
      <a href="https://github.com/alvdelci" target="_blank" rel="noopener">Link para meu GitHub</a>.
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h2 {
  color: purple;
}

h3 {
  font-size: 1.2rem;
}

a {
  text-decoration: underline;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
