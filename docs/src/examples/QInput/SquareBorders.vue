<template>
  <div class="q-pa-md">
    <div class="q-gutter-y-md column" style="max-width: 300px">
      <q-input square filled v-model="text">
        <template v-slot:prepend>
          <q-icon name="event" />
        </template>
      </q-input>

      <q-input square outlined v-model="text">
        <template v-slot:append>
          <q-avatar>
            <img src="https://cdn.efuzy.dev/logo/svg/efuzy-logo.svg">
          </q-avatar>
        </template>
      </q-input>

      <q-input square standout bottom-slots v-model="text" label="Label" counter>
        <template v-slot:prepend>
          <q-icon name="place" />
        </template>
        <template v-slot:append>
          <q-icon name="close" @click="text = ''" class="cursor-pointer" />
        </template>

        <template v-slot:hint>
          Field hint
        </template>
      </q-input>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      text: ''
    }
  }
}
</script>
