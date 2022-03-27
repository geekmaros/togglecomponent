<template>
<div :class="toggleState ? 'bg-gray-700': 'bg-white'" class="flex h-screen transition-all duration-500 ease-in-out justify-center items-center pt-12">
<!--  <ToggleVue2 v-model="toggleState" />-->
  <ToggleVue3 v-model="toggleState" />
  <span>Vue 3</span>
</div>
</template>
<script setup>
import {ref} from "vue";
import ToggleVue3 from "./components/ToggleVue3.vue";
const toggleState = ref(false)
</script>
<!--<script>-->
<!--import ToggleVue2 from "./components/ToggleVue2.vue";-->
<!--import ToggleVue3 from "./components/ToggleVue3.vue";-->
<!--export default {-->
<!--  components: {ToggleVue3, ToggleVue2},-->
<!--  data(){-->
<!--    return{-->
<!--      toggleState: false-->
<!--    }-->
<!--  }-->
<!--}-->
<!--</script>-->
<style>

</style>
