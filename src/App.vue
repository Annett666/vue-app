<template>
  <RegisterForm/>
</template>

<script>

import RegisterForm from "@/components/RegisterForm";
import {onBeforeMount, onMounted} from "vue";
export default {
  name: 'App',
  components: {
    RegisterForm,
  },
  setup() {
    onBeforeMount(() => {
      console.log('before mount')
    })
    onMounted(() => {
      console.log('mounted')
    })
  }
}
</script>

<style>
#app {
  font-family: 'Poppins', 'Arial', sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
p {
  margin: 0;
}
</style>
