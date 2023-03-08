<template>
  <q-page class="bg-grey-3 column">
    <q-list separator bordered>
      <q-item v-for="task in tasks" :key="task.title" v-ripple>
        <q-item-section avatar>
          <q-checkbox v-model="task.done" val="teal" color="primary" />
        </q-item-section>
        <q-item-section>
          <q-item-label>{{ task.title }}</q-item-label>
        </q-item-section>
      </q-item>
    </q-list>
  </q-page>
</template>

<script>
export default {
  data() {
    return {
      tasks: [
        {
          title: "hello",
          done: true,
        },
        {
          title: "hello2",
          done: false,
        },
        {
          title: "hello3",
          done: false,
        },
      ],
    };
  },
};
</script>
