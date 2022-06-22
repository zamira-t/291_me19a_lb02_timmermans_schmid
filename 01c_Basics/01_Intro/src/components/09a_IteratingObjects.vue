<template>
  <div>
    <h1>Starbucks</h1>
    <ul>
      <li v-for="n in 5" :key="n">
        <a href="#" @click="triggerAlert(n)">Drink {{ n }}</a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  methods: {
    triggerAlert(n) {
      alert(`${n} has been clicked`)
    },
  },
}
</script>

<style lang="scss" scoped>
ul {
  padding-left: 0;
}
li {
  display: block;
  list-style: none;

  + li {
    margin-top: 10px;
  }
}

h1 {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  font-size: 40px;
}

a {
  display: inline-block;
  background: #00991e;
  border-radius: 20px;
  color: white;
  padding: 10px 20px;
  text-decoration: none;
}
</style>
