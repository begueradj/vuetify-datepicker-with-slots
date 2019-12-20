<template>
  <div>
    <main>
      <slot v-bind:myName="myName" />
    </main>
    <p> Page component </p>
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
