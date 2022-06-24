<template>
  <div>
    {{ pending ? 'Loading' : count }}
  </div>
</template>

<script setup>
const { pending, data: count } = useLazyAsyncData('count', () => $fetch('https://jsonplaceholder.typicode.com/posts/1'))
watch(count, (newCount) => {
  // Because count starts out null, you won't have access
  // to its contents immediately, but you can watch it.
})
</script>