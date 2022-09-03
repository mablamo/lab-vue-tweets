<script setup>

const props = defineProps({
  image: String,
})
</script>

<template>

    <img
      :src="props.image"
      className="profile"
      alt="profile"
    />

</template>