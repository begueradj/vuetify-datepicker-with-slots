<template>
  <page-component>
    <template v-slot="{ myName }">
      <v-btn> {{ myName }} </v-btn>
    </template>
  </page-component>
</template>

<script>
import PageComponent from '@/components/PageComponent.vue'
export default {
  components: { PageComponent }
}
</script>
