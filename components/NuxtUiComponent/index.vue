<script setup lang="ts">
const nuxtUiComponents = ref<string[]>([
  'accordion',
  'alert',
  'badge',
  'breadcrumb',
  'button',
  'card',
  'carousel',
  'checkbox',
  'chip',
  'command-palette',
  'container',
  'context-menu',
  'date-picker',
  'divider',
  'dropdown',
  'form',
  'form-group',
  'horizontal-navigation',
  'icon',
  'input',
  'input-menu',
  'kbd',
  'link',
  'meter',
  'modal',
  'notification',
  'pagination',
  'popover',
  'progress',
  'radio-group',
  'range',
  'select',
  'select-menu',
  'skeleton',
  'slideover',
  'table',
  'tabs',
  'textarea',
  'toggle',
  'tooltip',
  'vertical-navigation',
])
</script>

<template>
  <div class="box">
    <div v-for="item in nuxtUiComponents" :key="item" class="box__item">
      <div class="box__item__title">{{ item.replace("-", " ") }}</div>
      <component :is="`nuxt-ui-component-${item}`" />
    </div>
  </div>
</template>

<style lang="postcss" scoped>
.box {
  @apply flex flex-col items-start justify-normal gap-8;
  @apply w-full;
  &__item {
    @apply w-full;
    &__title {
      @apply text-xl font-bold mb-2 capitalize;
    }
  }
}
</style>
