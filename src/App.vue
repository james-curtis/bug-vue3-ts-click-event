<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
function onClickHandler(e: MouseEvent) {
  console.log('click', e);
}
function onDblclick(e: MouseEvent) {
  console.log('dblclick', e);
}
</script>

<template>
  <div>
    <a target="_blank" @click="onClickHandler">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
