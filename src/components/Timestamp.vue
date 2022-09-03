<script setup>

const props = defineProps({
  time: String,
})
</script>

<template>

    <span className="timestamp">{{time}}</span>

</template>