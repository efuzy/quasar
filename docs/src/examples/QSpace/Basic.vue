<template>
  <div class="q-pa-md">
    <q-toolbar class="bg-primary text-white">
      <q-btn flat round dense icon="menu" />

      <q-space />

      <q-btn flat round dense icon="apps" class="q-mr-xs" />
      <q-btn flat round dense icon="more_vert" />
    </q-toolbar>

    <div class="row no-wrap items-center q-mt-md q-pa-sm bg-grey-3 rounded-borders">
      <q-avatar>
        <img src="https://cdn.efuzy.dev/logo/svg/efuzy-logo.svg">
      </q-avatar>

      <q-space />

      <div>
        Efuzy <q-badge>v{{ $q.version }}</q-badge>
      </div>
    </div>
  </div>
</template>
