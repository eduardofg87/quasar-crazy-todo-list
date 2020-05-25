<template>
  <q-page class="bg-grey-3 column">
    <q-list>

      <q-item
        v-for="task in tasks"
        :key="task.title"
        v-ripple>
        <q-item-section avatar>
          <q-checkbox
            v-model="color"
            color="primary" />
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
  data () {
    return {
      tasks: [
        {
          title: 'Get bananas',
          done: false
        },
        {
          title: 'Eat bananas',
          done: false
        },
        {
          title: 'Poo bananas',
          done: false
        }
      ]
    }
  }
}
</script>
