<template>
  <div>
    <h1>{{ reactiveData }}</h1>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from '@nuxtjs/composition-api'

export default defineComponent({
  name: 'Home',
  setup() {
    const reactiveData = ref('this is composed')

    return {
      reactiveData,
    }
  },
})
</script>

<style lang="stylus" scoped></style>
