<template>
  <div>
    {{ pending ? 'Loading' : count }}
  </div>
</template>

<script setup>
const { pending, data: count } = useLazyAsyncData('count', () => $fetch('/api/hello'))
watch(count, (newCount) => {
  // Because count starts out null, you won't have access
  // to its contents immediately, but you can watch it.
})
</script>