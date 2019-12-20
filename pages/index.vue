<template>
  <div>
    <page-component>
      <template v-slot="{ myName }">
        <v-btn> {{ myName }} </v-btn>
      </template>
      <template #begueradj>
        <date-picker-slot v-slot="{ dateFormatted }" />
        <v-btn> {{ dateFormatted }} </v-btn>
      </template>
    </page-component>
  </div>
</template>

<script>
import PageComponent from '@/components/PageComponent.vue'
import DatePickerSlot from '@/components/DatePickerSlot.vue'

export default {
  components: { PageComponent, DatePickerSlot }
}
</script>
