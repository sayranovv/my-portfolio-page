<script setup lang="ts">

</script>

<template>
  <div class="h-screen p-8">
    <div class="p-8 border border-gray-700 h-full overflow-hidden">
      <LayoutHeader class="w-full" />
      <div class="h-full mt-16">
        <div class="absolute">
          <LayoutMenu />
        </div>
        <div class="absolute bottom-20 right-20">
          <Transition name="fade" mode="out-in">
            <slot />
          </Transition>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.fade-enter-active, .fade-leave-active {
  transition: opacity 0.5s;
}

.fade-enter-from, .fade-leave-to {
  opacity: 0;
}
</style>