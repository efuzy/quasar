<template>
  <div class="q-pa-md">
    <q-responsive :ratio="16/9" style="width: 500px; max-width: 100%;">
      <q-carousel
        swipeable
        animated
        arrows
        v-model="slide"
        infinite
      >
        <q-carousel-slide :name="1" img-src="https://cdn.efuzy.dev/img/mountains.jpg" />
        <q-carousel-slide :name="2" img-src="https://cdn.efuzy.dev/img/parallax1.jpg" />
        <q-carousel-slide :name="3" img-src="https://cdn.efuzy.dev/img/parallax2.jpg" />
        <q-carousel-slide :name="4" img-src="https://cdn.efuzy.dev/img/efuzy.jpg" />

        <template v-slot:control>
          <q-carousel-control
            position="bottom"
            :offset="[16, 8]"
            class="text-white text-center rounded-borders"
            style="background: rgba(255, 255, 255, .2); padding: 4px 8px;"
          >
            Ratio 16:9
          </q-carousel-control>
        </template>
      </q-carousel>
    </q-responsive>
  </div>
</template>

<script>
export default {
  data () {
    return {
      slide: 1
    }
  }
}
</script>
