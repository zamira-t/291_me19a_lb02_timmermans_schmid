<template>


  <div>
    <h1>Starbucks </h1>


    <h3>Drinks:</h3>
    <ul>
      <li v-for="n in drinks" :key="n">
        {{n.title}}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      interests: ['Drinks Cold', 'Drinks Warm', 'Snacks'],
      drinks: [
          {
            title: 'Cappuccino',
          },{
            title: 'Frappuccino',
          },
        {
          title: 'Iced Caffée',
        },
        {
          title: 'Caramel Cappuccino',
        },
      ]
    }
  },
}
</script>

<style lang="scss" scoped>
li {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  color: #2c3e50;
  margin-top: 50px;
}

h1 {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  color: #3d9137;
  margin-top: 60px;
}

  h3 {
    color: #a04db3;
  }
</style>
