<template>
  <div>
      <Input @changeWord="changer"/>
      
      <section>
      
      </section>
    </div>
</template>

<script setup>
import {ref} from 'vue';
import Input from './components/InputComponent.vue';

const theWord=ref('');

function changer(value){
    theWord.value=value;
}

</script>



<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
 }
#app{
    background:skyblue;
    height:100vh;
    padding-top: 20vh;
    display:flex;
    justify-content:center;
    }
</style>
