<template>
  <div>
    <slot v-bind:myName="myName" />
    <slot name="begueradj" />
    <p> This belongs to page component and can not be modified by parent component </p>
  </div>
</template>

<script>
export default {
  name: 'PageComponent',
  data () {
    return {
      myName: 'Begueradj',
      country: 'France'
    }
  }
}
</script>
