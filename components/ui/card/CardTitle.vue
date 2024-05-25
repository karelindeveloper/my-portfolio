<script setup lang="ts">
import { cn } from '@/lib/utils'
import type { HTMLAttributes } from 'vue'

const props = defineProps<{
  class?: HTMLAttributes['class']
}>()
</script>

<template>
  <h6 :class="cn('font-medium text-accent-foreground text-2xl lg:text-[32px] leading-normal lg:leading-normal', props.class)
    ">
    <slot />
  </h6>
</template>
