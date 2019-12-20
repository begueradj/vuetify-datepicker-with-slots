<template>
  <div>
    <!-- <page-component>
      <template v-slot="{ myName }">
        <v-btn> {{ myName }} </v-btn>
      </template>
      <template #begueradj>
        <p> Named slot in page component filled by parent component </p>
      </template>
    </page-component>
    <named-slot-with-variable>
      <template v-slot="{avecNom, country } ">
        {{ country }}
      </template>
    </named-slot-with-variable>
    Correct way:
    <named-slot-with-variable>
  <template v-slot:withName=" { country } ">
    {{ country }}
  </template>
</named-slot-with-variable>
    -->
    <date-picker-slot>
      <template v-slot=" { dateFormatted } ">
        <v-btn> {{ dateFormatted }} </v-btn>
      </template>
    </date-picker-slot>
  </div>
</template>

<script>
// import PageComponent from '@/components/PageComponent.vue'
import DatePickerSlot from '@/components/DatePickerSlot.vue'
// import NamedSlotWithVariable from '@/components/NamedSlotWithVariable.vue'

export default {
  components: { DatePickerSlot }
}
</script>
