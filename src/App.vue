<script setup>
import TheWelcome from '@/components/pages/TheWelcome.vue'
import Layout from '@/components/layouts/Layout.vue'
import TheDashboard from '@/components/pages/TheDashboard.vue'
import TheWorkout from '@/components/pages/TheWorkout.vue'
import { ref } from 'vue'

const selectedDisplay = ref(3)
</script>

<template>
  <Layout>
    <!--PAGE 1-->
    <TheWelcome v-if="selectedDisplay === 1" />
    <!--PAGE 2-->
    <TheDashboard v-if="selectedDisplay === 2" />
    <!--PAGE 3-->
    <TheWorkout v-if="selectedDisplay === 3" />
  </Layout>
</template>

<style scoped></style>
