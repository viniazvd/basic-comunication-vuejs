<template>
  <div>
    Meu time é: {{ time }}

    <br>
     
    <input :value="this.time" @input="this.filhoEnviaTime" />
  </div>
</template>

<script>
export default {
  props: ['time'],

  methods: {
    filhoEnviaTime () {
      const newValue = event.target.value
      this.$emit('update:time', newValue)
    }
  }
}
</script>
