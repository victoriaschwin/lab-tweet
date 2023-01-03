<template>
          <span className="name">{{ name }}</span>
          <span className="handle">{{ handle }}</span>

</template>

<script setup>
const props = defineProps(["name", "handle"]);
</script>

<style>

</style>