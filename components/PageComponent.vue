<template>
  <div>
    <slot v-bind:myName="myName" />
    <p> Page component </p>
    <slot name="begueradj" />
  </div>
</template>

<script>
export default {
  name: 'PageComponent',
  data () {
    return {
      myName: 'Begueradj'
    }
  }
}
</script>
