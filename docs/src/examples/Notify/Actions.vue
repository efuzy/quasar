<template>
  <div class="q-pa-md">
    <q-btn color="purple" @click="showNotif" label="Show Notifications" />
  </div>
</template>

<script>
export default {
  methods: {
    showNotif () {
      this.$q.notify({
        message: 'Jim just pinged you.',
        color: 'primary',
        avatar: 'https://cdn.efuzy.dev/img/boy-avatar.png',
        actions: [
          { label: 'Dismiss', color: 'white', handler: () => { /* ... */ } }
        ]
      })

      this.$q.notify({
        message: 'Jim just pinged you.',
        color: 'primary',
        avatar: 'https://cdn.efuzy.dev/img/boy-avatar.png',
        actions: [
          { label: 'Reply', color: 'yellow', handler: () => { /* ... */ } },
          { label: 'Dismiss', color: 'white', handler: () => { /* ... */ } }
        ]
      })
    }
  }
}
</script>
