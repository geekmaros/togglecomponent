<template>
<div :class="modelValue ? 'bg-orange-500' : 'bg-gray-300'" @click="toggle" class="w-14 transition-all duration-500 h-8 flex items-center bg-gray-300 rounded-full p-1">
  <div :class="{'translate-x-6': modelValue}" class="w-6 h-6 transition-all duration-500 transform bg-white rounded-full shadow-md"></div>
</div>
</template>

<script>
export default {
  name: "ToggleVue2",
  props:{
    modelValue: {
      type: Boolean,
    }
  },
  methods: {
    toggle(){
      console.log(!this.modelValue)
      this.$emit('update:modelValue', !this.modelValue)
    }
  }
}
</script>

<style scoped>

</style>
