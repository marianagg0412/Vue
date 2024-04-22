<template>
    <h1> {{title || "Nameless"}}</h1>
    <p> {{ counter }} </p>
    <button @click="increment">+1</button>
    <button @click="decrement">-1</button>
</template>

<script>
export default {
    props: ['title'],
    data(){
        return{
            counter: 0
        }
    },
    methods:{
        increment(){
            this.counter++;
        },
        decrement(){
            this.counter--;
        }
    }
}
</script>

<style>
</style>