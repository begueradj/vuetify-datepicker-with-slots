<template>
  <div>
    <slot v-bind:country="{ country }" name="avecNom" />
    Named slot with variable
  </div>
</template>

<script>
export default {
  name: 'NamedSlotWithVariable',
  data () {
    return {
      country: 'France'
    }
  }
}
</script>
