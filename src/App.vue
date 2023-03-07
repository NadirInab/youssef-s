<template>
  <header>
      <!-- <Greet title="Nadfir" /> -->
      <Greet @youssef="showme" @test="showData"  :title="title" />
      <!-- <Test v-show="show" test="tesing here baby" /> -->
  </header>
</template>

<script >
import Greet from "./components/Greet.vue" ;
import Test from "./components/Test.vue" ;

export default {
  data(){
    return {
      show : true, 
      title : "Nadir"
    }
  },
  components : {
    Greet, 
    Test 
  }, 
  methods : {
    showData(){
      // console.log(data) ;
      this.title = "youssef test"
    }, 
    showme(data){
      console.log(data) ;
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
