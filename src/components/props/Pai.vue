<template>
  <div>

    <p><strong>Exemplo com props simples:</strong></p>
    
    <Filho :propTime="time"></Filho>
    
    <br>

    <p><strong>Exemplo com props dinâmicas (v-model):</strong></p>
    <input v-model="time">

    <br>
    <br>

  </div>
</template>

<script>
import Filho from './Filho'

export default {
  components: { Filho },

  data () {
    return {
      time: 'Mengão'
    }
  }
}
</script>
