<template>
  <UTable
    sort-asc-icon="i-heroicons-arrow-up-20-solid"
    sort-desc-icon="i-heroicons-arrow-down-20-solid"
    :sort-button="{
      icon: 'i-heroicons-sparkles-20-solid',
      color: 'primary',
      variant: 'outline',
      size: '2xs',
      square: false,
      ui: { rounded: 'rounded-full' },
    }"
    class="w-full"
    :columns="[
      { key: 'id', label: 'ID' },
      { key: 'name', label: 'Name', sortable: true },
      { key: 'title', label: 'Title', sortable: true },
      { key: 'email', label: 'Email', sortable: true },
      { key: 'role', label: 'Role' },
    ]"
    :rows="[
      {
        id: 1,
        name: 'Lindsay Walton',
        title: 'Front-end Developer',
        email: 'lindsay.walton@example.com',
        role: 'Member',
      },
      {
        id: 2,
        name: 'Courtney Henry',
        title: 'Designer',
        email: 'courtney.henry@example.com',
        role: 'Admin',
      },
      {
        id: 3,
        name: 'Tom Cook',
        title: 'Director of Product',
        email: 'tom.cook@example.com',
        role: 'Member',
      },
      {
        id: 4,
        name: 'Whitney Francis',
        title: 'Copywriter',
        email: 'whitney.francis@example.com',
        role: 'Admin',
      },
      {
        id: 5,
        name: 'Leonard Krasner',
        title: 'Senior Designer',
        email: 'leonard.krasner@example.com',
        role: 'Owner',
      },
      {
        id: 6,
        name: 'Floyd Miles',
        title: 'Principal Designer',
        email: 'floyd.miles@example.com',
        role: 'Member',
      },
    ]"
  />
</template>
