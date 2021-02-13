<template>
  <div>
    <div class="count">{{ count }}</div>
    <button class="increment" @click="increment">Жми, чтоб прибавить</button>
    <button class="decrement" @click="decrement">Жми, чтоб убавить</button>
  </div>
</template>

<script>
export default {
  name: 'Counter',
  data() {
    return {
      // Инициализируем с нуля
      count: 0,
    }
  },
  methods: {
    increment() {
      this.count += 1;
    },
    decrement() {
      this.count -= 1;
    }
  }
}
</script>

<style scoped>
button{
  border-radius: 20%;
  height: 70px;
  width: 85px;
  outline: none;
  border:none;
  font-weight: 700;
  font-family: "Roboto", sans-serif;
}

.increment{
  background-color: green;
}

.decrement{
  background-color: red;
  margin-left: 30px;
}

.count{
  margin: 20px auto 20px;
  display: block;
  width: 50px;
  font-size: 30px;
  font-weight: 700;
  border:2px solid black;
  padding: 10px;
}
</style>