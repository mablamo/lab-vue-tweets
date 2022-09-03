<script setup>

const props = defineProps({
  userData: Object,
})
</script>

<template>
    <span className="user">
          <span className="name">{{props.userData.name}}</span>
          <span className="handle">{{props.userData.handle}}</span>
    </span>
</template>
