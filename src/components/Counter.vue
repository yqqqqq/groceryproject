<template>
  <div>
      <input type="button" v-bind:value="decrement_text" v-on:click="decrementCounter">
      {{counter}}
      <input type="button" v-bind:value="increment_text" v-on:click="incrementCounter">
  </div>
</template>

<script>
export default {
  data(){
    return{
        decrement_text: "-",
        counter: 0,
        increment_text: "+",
        }
  },
  methods: {
      decrementCounter: function() {
          this.counter=this.counter-1
      },
      incrementCounter: function() {
          this.counter=this.counter+1
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>