<template>
  <div>
    <button @click="filhoEnviaTime">Qual o seu time?</button>
    <button @click="filhoZeraTime">Limpar nome time</button>
  </div>
</template>

<script>
export default {
  methods: {
    filhoEnviaTime () {
      this.$emit('escutandoEventoDoFilhoPerguntandoTime')
    },

    filhoZeraTime () {
      this.$emit('escutandoEventoDoFilhoZerandoTime')
    }
  }
}
</script>
