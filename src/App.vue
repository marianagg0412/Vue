<template>
  <CounterAppVue title="nom nom nom nom nom nom nom nom nom"/>
  <CounterAppVue title="Juan el amor de Julio"/>
</template>

<script>

import CounterAppVue from './components/CounterApp.vue'
export default {
  name: 'App',
  components: {
    CounterAppVue
  },
  data(){ //data is used to store the data
    return{
      food: ['Pizza', 'Burger', 'Pasta'],
      name: '',
      counter: 5
    }
  },
  methods:{ //methods are used to add functionality to the app
    addElement(){
      this.food.push(this.name);
      this.name = '';
    }
  },
  computed:{ //computed is used to calculate the data
    squareComputed(){
      return this.counter*this.counter;
    }
  }
}
</script>

<style>
  button{
    background-color: #64b687;
    border-radius: 5px;
    border: 1px solid white;
    color: white;
    cursor: pointer;
    margin: 0 5px;
    padding: 5px 15px;
    transition: 0.3 ease-in-out;
  }
  button:hover{
    background-color: #6465b6;
    transition: 0.3s ease-in-out;
  }

</style>
