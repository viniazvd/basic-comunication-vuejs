<template>
  <div>

    <p><strong>Exemplo bileteral de evento filho-pai (com .sync):</strong></p>

    <Filho :time.sync="time"></Filho>

    <br>

    <p><strong>Exemplo bileteral de evento filho-pai (suportando v-model):</strong></p>

    Pai pergunta: "Filho, qual o meu time?" <input v-model="time">

  </div>
</template>

<script>
import Filho from './Filho'

export default {
  components: { Filho },

  data () {
    return {
      time: ''
    }
  }
}
</script>
