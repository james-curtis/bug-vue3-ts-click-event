<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
function onClickHandler(e: MouseEvent) {
  /**
   * TODO: `e` would be PointerEvent
   * vscode with volar report:
   * `(property) click: ((payload: MouseEvent) => void) | undefined`
   * @link https://www.w3.org/TR/uievents/#event-types-list
   */
  console.log('click', e);
}

function onDblclick(e: MouseEvent) {
  // it's right. MouseEvent
  // @link https://www.w3.org/TR/uievents/#event-types-list
  console.log('dblclick', e);
}
</script>

<template>
  <div>
    <div @click="onClickHandler">
      <img src="/vite.svg" class="logo" alt="Vite logo"/>
    </div>
    <div @dblclick="onDblclick">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo"/>
    </div>
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
