<template>
  <header
    class="el-header"
    :style="{ height }"
  >
    <slot />
  </header>
</template>

<script setup lang="ts">
import {withDefaults} from 'vue'

interface Props {
  height:string
}
withDefaults(defineProps<Props>(),{
  height:"60px"
})

</script>

<style lang="scss">
@import '../styles/mixin';

</style>