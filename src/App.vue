<script setup>
import {ref, computed} from "vue";

const counter = ref(0);

const add = ( ) => counter.value++ 

const rest = ( ) => counter.value--

const reset =() => (counter.value = 0)


</script>

<template>
  <h1>Counter</h1>
  <p>{{ counter }}</p>
  <button v-on:click="add">Add</button>
  <button @:click="rest">Rest</button>
  <button v-on:click="reset">Reset</button>
</template>

<style>
h1 {
  color: green;
}
</style>
