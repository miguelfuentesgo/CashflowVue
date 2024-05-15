<template>
  <Suspense>
    <template #default>
      <Home />
    </template>
    <template #fallback>
      <SplashScreen />
    </template>
  </Suspense>
</template>

<script setup>
import SplashScreen from "./pages/SplashScreen";
import { defineAsyncComponent } from "vue";

const Home = defineAsyncComponent(
  () =>
    new Promise((resolve) => {
      setTimeout(() => resolve(import("./pages/Home")), 2000);
    })
);
</script>
