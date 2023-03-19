<template>
  <TheNavigation />
  <div class="container">
    <router-view> </router-view>
  </div>
</template>

<script>
import TheNavigation from "@/components/TheNavigation.vue";
export default {
  components: { TheNavigation },
};
</script>

<style>
.slide-enter-active,
.slide-leave-active {
  transition: opacity 1s, transform 1s;
}

.slide-enter-from,
.slide-leave-to {
  opacity: 0;
  transform: translateX(-30%);
}
</style>
