<script setup>
defineProps({
  text: String,
  icon: Object
})
</script>

<template>
  <div class="inline-flex items-center gap-2 px-4 py-1 rounded-full bg-purple-100 text-purple-600 text-sm">
    
    <!-- ICON BISA DIGANTI -->
    <component :is="icon" class="w-4 h-4" />

    {{ text }}
  </div>
</template>

<!-- <script setup lang="ts">--
defineProps<{
  text: string
  variant?: 'primary' | 'secondary'
}>()
</script>

<template>
  <span
    class="inline-flex items-center px-4 py-1.5 rounded-full text-xs font-semibold tracking-wider uppercase"
    :class="[
      variant === 'secondary'
        ? 'bg-gray-100 text-gray-600 border border-gray-200'
        : 'bg-gradient-to-r from-purple-100 to-pink-100 text-purple-700 border border-purple-200'
    ]"
  >
    {{ text }}
  </span>
</template>-->
