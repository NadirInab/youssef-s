<template>
  <div>
    <h1>Hello from {{title}}</h1>
    <button @click="$emit('test')">click</button>
    <button @click="$emit('youssef', 'tesing lfdmfjgksdfml')"></button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "Nadir"
    };
  },
  methods : {
    changeName(){
        this.name = "Yousszef"
    }
  }, 
  props : {
    title : String
  }
};
</script>

<style>
</style>