<script setup>
defineProps(
    {
      lists:Array
    }

)

</script>

<template>
  <div class="grid grid-flow-row grid-cols-3 gap-4 mb-2">
    <template v-for="(list,index) in lists" :key="index" >
    <a :class="list.tags[0].class" class="mx-auto" href="/11r/tag/cats">{{list.tags[0].name}}</a>
    </template>
  </div>

</template>

<style scoped>

</style>