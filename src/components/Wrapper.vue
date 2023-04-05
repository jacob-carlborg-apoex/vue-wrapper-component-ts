<template>
  <Child v-bind="$attrs">
    <template
      v-for="(name, index) of Object.keys($slots)"
      #[name]="slotData"
      :key="index"
    >
      <slot :name="name" v-bind="slotData || {}"></slot>
    </template>
  </Child>
</template>

<script setup lang="ts">
import Child from '@/components/Child.vue'
</script>

<script lang="ts">
export default {
  inheritAttrs: false
}
</script>
