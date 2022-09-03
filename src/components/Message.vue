<script setup>

const props = defineProps({
  message: String,
})
</script>

<template>

      <p className="message">
        {{message}}
      </p>

</template>