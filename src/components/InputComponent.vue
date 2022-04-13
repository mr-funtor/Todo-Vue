<template>
  <input type="text" v-model="text" @input="sendUp"/>
</template>

<script setup>
import{ref} from 'vue';

const text=ref('');

const emit= defineEmits(['changeWord']);
function sendUp(){
    emit('changeWord',text.value);
}

</script>



<style scoped>

</style>
