<template>
  <div>
    <page-component>
      <template v-slot="{ myName }">
        <v-btn> {{ myName }} </v-btn>
        <h1> Some text </h1>
      </template>
      <template #begueradj>
        Named slot
      </template>
    </page-component>
  </div>
</template>

<script>
import PageComponent from '@/components/PageComponent.vue'
export default {
  components: { PageComponent }
}
</script>
