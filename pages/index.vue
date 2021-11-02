<template>
  <div id="counter">
  <h3>Counter: {{ counter }}</h3>
  <button type="button" v-on:click="increase">Increase</button> 
  <p></p>
  <button type="button" v-on:click="decrease">Decrease</button> 

</div>
</template>

<script>
export default {

  data() {
    return {
               counter: 0            
      }       
    
  },
  methods: {
    increase: function() {
      this.counter++;
    },
    decrease: function() {
      this.counter--;
    }
  }
}
</script>
