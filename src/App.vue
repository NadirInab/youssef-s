<template>
  <header>
      <!-- <Greet title="Nadfir" /> -->
      <Greet @changeName="showData"  title="Youssef" />
      <Test v-show="show" test="tesing here baby" />
  </header>
</template>

<script >
import Greet from "./components/Greet.vue" ;
import Test from "./components/Test.vue" ;

export default {
  data(){
    return {
      show : true
    }
  },
  components : {
    Greet, 
    Test
  }, 
  methods : {
    showData(data){
      console.log(data) ;
      this.show = !this.show
    }
  }
}
</script>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
