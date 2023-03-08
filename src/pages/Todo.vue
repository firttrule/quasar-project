<template>
  <q-page class="q-pa-lg">
    <h5>Todo</h5>

    <div class="q-pa-md" style="max-width: 350px">
      <q-list bordered separator>
        <q-item clickable v-ripple>
          <q-item-section>first todo</q-item-section>
        </q-item>

        <q-item clickable v-ripple>
          <q-item-section>
            <q-item-label>second todo</q-item-label>
            <q-item-label caption>done</q-item-label>
          </q-item-section>
        </q-item>

        <q-item clickable v-ripple>
          <q-item-section>
            <q-item-label>third todo</q-item-label>
          </q-item-section>
        </q-item>
      </q-list>
    </div>
  </q-page>
</template>

<script>
</script>
