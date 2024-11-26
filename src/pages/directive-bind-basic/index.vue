<script setup lang="ts">
import { ref } from "vue";

defineOptions({
  name: "DirectiveBindBasic",
});

const url = ref("https://vuejs.org/");
const GUIDE_PATH = "guide/introduction.html";
</script>

<template>
  <div class="directive-bind-basic">
    <p>
      <a v-bind:href="url" target="_blank"> Vue.js(v-bind) </a>
    </p>
    <p>
      <a :href="url" target="_blank"> Vue.js(省略記法) </a>
    </p>
    <p>
      <a :href="`${url}${GUIDE_PATH}`" target="_blank">
        Vue.js(テンプレートリテラル)
      </a>
    </p>
  </div>
</template>
