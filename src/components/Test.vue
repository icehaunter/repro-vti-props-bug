<template>
  <pre>{{ test }}</pre>
</template>

<script lang="ts">
import { defineComponent, PropType } from 'vue'

interface TestInterface {
  key: string
}

export default defineComponent({
  props: {
    test: { 
      type: Object as PropType<TestInterface>,
      required: false,
    }
  }
})
</script>
