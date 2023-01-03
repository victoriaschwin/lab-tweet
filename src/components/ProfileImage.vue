<template>
    <img
      :src="image"
      className="profile"
      alt="profile"
    />
</template>

<script setup>
const props = defineProps(["image"]);
</script>
