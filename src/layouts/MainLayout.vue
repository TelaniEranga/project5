<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>

    </q-header>
    <q-toolbar class="bg-primary text-white bg-black  shadow-2">
      <q-btn flat round dense icon="menu" class="q-mr-sm" />
      <q-separator dark vertical inset />
      <q-btn stretch flat label="Link" />

      <q-space />

      <q-separator dark vertical />
      <q-btn stretch flat label="About" a href="HomePage.Vue" />
      <q-separator dark vertical />
      <q-btn stretch flat label="Contact Us" />
    </q-toolbar>
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>

</script>
