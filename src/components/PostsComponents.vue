<script setup>
defineProps(
    {
      posts:Array,
    }
)
</script>

<template>
<span v-for="(post,index) in posts" :key="index" >

  <div class="mb-8 border-dotted border-b pb-8 border-gray-300">
    <h2>
      <a class="block" href="/11r/post/deadbeef-decrementation/">{{post.title}}</a>
    </h2>

    <p class="excerpt">{{post.excerpt}}</p>

    <a :class="post.tags[0].class" href="/11r/tag/spirituality">{{post.tags[0].name}}</a>
    <a :class="post.tags[1].class" href="/11r/tag/spirituality">{{post.tags[1].name}}</a>

    <span class="block md:inline md:float-right md:pt-4 pt-2 created-date" datetime="Sat Oct 08 2016 19:00:00 GMT-0500 (Central Daylight Time)">
            October 9, 2016
          </span>
  </div>

</span>
</template>

<style scoped>

</style>