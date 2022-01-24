<template>
  <div class="home">
    <div class="counter">
      {{ counter }}
    </div>
    <div class="buttons">
      <button @click="decreaseCounter">-</button>
      <button @click="increaseCounter">+</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      counter: 0,
    };
  },
  methods: {
      increaseCounter(){
          this.counter ++
      },
    decreaseCounter(){
          this.counter --
      },
  },
};
</script>

<style scoped>
div {
  margin-bottom: 2rem;
}
.counter {
  font-size: 50px;
}
button {
  margin: 1rem;
  width: 3rem;
  font-size: 2rem;
}
</style>