<template>
  <q-page class="q-pa-lg">
    <h5>Kitties carousel</h5>
    <div class="q-pa-md">
      <q-carousel
        animated
        v-model="slide"
        arrows
        navigation
        infinite
        style="width: 400px; height: 400px"
      >
        <q-carousel-slide :name="1" img-src="../assets/cat2.jpg" />
        <q-carousel-slide :name="2" img-src="../assets/cat3.png" />
        <q-carousel-slide :name="3" img-src="../assets/cat4.jpg" />
        <q-carousel-slide :name="4" img-src="../assets/cat5.jpg" />
      </q-carousel>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
import { ref } from "vue";

export default defineComponent({
  name: "IndexPage",
  setup() {
    return {
      slide: ref(1),
    };
  },
});
</script>
