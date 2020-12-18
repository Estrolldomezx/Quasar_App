<template>
  <div class="q-pa-md">
    <q-option-group
      v-model="controlType"
      :options="controlTypeOptions"
      color="purple"
      inline
      class="q-mb-md"
    />
    <q-carousel
      v-model="slide"
      swipeable
      animated
      :control-type="controlType"
      control-color="purple"
      navigation
      padding
      arrows
      height="80vh"
      class="text-purple rounded-borders"
    >
      <q-carousel-slide :name="1" img-src="https://cdn.quasar.dev/img/mountains.jpg">
      </q-carousel-slide>
      <q-carousel-slide :name="2" img-src="https://cdn.quasar.dev/img/parallax1.jpg">
      </q-carousel-slide>
      <q-carousel-slide :name="3" img-src="https://cdn.quasar.dev/img/parallax2.jpg">
      </q-carousel-slide>
      <q-carousel-slide :name="4" img-src="https://cdn.quasar.dev/img/quasar.jpg" >
      </q-carousel-slide>
    </q-carousel>
  </div>
</template>

<script>
export default {
  name: 'PageIndex',
  data () {
    return {
      slide: 1
    }
  }
}

</script>
