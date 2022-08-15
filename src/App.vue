<script setup lang="ts">
import { RouterView, RouterLink } from 'vue-router';
</script>

<template>
  <ul>
    <li><RouterLink to="/"></RouterLink></li>
    <li><RouterLink to="/login"></RouterLink></li>
  </ul>
  <RouterView />
</template>
