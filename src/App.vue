<template>
  <Wrapper>
    <template v-slot:foo>Foo</template>
    <template v-slot:bar>Bar</template>
  </Wrapper>
</template>

<script setup lang="ts">
import Wrapper from '@/components/Wrapper.vue'
</script>