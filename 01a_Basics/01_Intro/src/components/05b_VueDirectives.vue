<template>


  <div>
    <h1 v-if="false" v-text="mytext">Loading...</h1>
    <h2 v-else-if="false" v-html="myhtml" />
    <a
            v-else
            :href="link.url"
            :target="link.target"
            :tabindex="link.tabindex"
            v-text="link.title"
    />
  </div>
</template>

<script>
  export default {
    data() {
      return {
        // v-text
        mytext: '05b_VueDirectives.vue (text)',
        // v-html
        myhtml: 'intro-5b </br>HTML in<br/><b>your data</b>',
        // v-bind
        link: {
          url: 'https://www.starbucks.ch/de',
          target: '_blank',
          tabindex: '0',
          title: 'Hier gehts zur Starbucks Webseite'
        },
      }
    },
  }
</script>


<style lang="scss" scoped>
h2 {
  margin: 40px;
  font-weight: normal;

}

a {
  display: block;
  margin-top: 100px;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  color: #055524;
  text-align: center;
  font-size: 40px;
}
</style>
