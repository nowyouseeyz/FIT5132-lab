<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      Github Link:
      <a href="https://github.com/mliu0102" target="_blank" rel="noopener">https://github.com/mliu0102</a>.
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
  color: blueviolet;
}

h3 {
  font-size: 1.2rem;

  a{
    color: aqua;
  }
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
