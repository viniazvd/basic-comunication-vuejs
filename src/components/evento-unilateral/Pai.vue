<template>
  <div>
    <p><strong>Exemplo unilateral de evento filho-pai:</strong></p>

    <Filho 
      @escutandoEventoDoFilhoPerguntandoTime="paiEscolheTime" 
      @escutandoEventoDoFilhoZerandoTime="paiZeraTime">
    </Filho>
    
    <p>Meu time é: {{ time }}</p>
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
  },

  methods: {
    paiEscolheTime () {
      this.time = 'Mengão !'
    },

    paiZeraTime () {
      this.time = ''
    }
  }
}
</script>
