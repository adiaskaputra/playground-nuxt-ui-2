<script setup lang="ts"></script>

<template>
  <div class="flex-horiz">
    <UAvatar
      src="https://avatars.githubusercontent.com/u/739984?v=4"
      alt="Avatar"
    />
    <UAvatar
      chip-color="primary"
      chip-text=""
      chip-position="top-right"
      size="sm"
      src="https://avatars.githubusercontent.com/u/739984?v=4"
      alt="Avatar"
    />
    <UAvatar icon="i-heroicons-photo" size="sm" />
    <UAvatarGroup size="sm" :max="2">
      <UAvatar
        src="https://avatars.githubusercontent.com/u/739984?v=4"
        alt="benjamincanac"
      />
      <UAvatar
        src="https://avatars.githubusercontent.com/u/904724?v=4"
        alt="Atinux"
      />
      <UAvatar
        src="https://avatars.githubusercontent.com/u/7547335?v=4"
        alt="smarroufin"
      />
    </UAvatarGroup>
  </div>
</template>

<style lang="scss" scoped></style>
