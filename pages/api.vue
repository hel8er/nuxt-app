<script setup>
const { data } = await useAsyncData('count', () => $fetch('https://jsonplaceholder.typicode.com/posts/1'))
</script>

<template>
<p>Full data: {{ data }}</p>
  id: <p>{{ data.id }}</p>
  <h1>{{ data.title }}</h1>
</template>