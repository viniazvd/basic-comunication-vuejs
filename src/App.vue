<template>
  <div>

    <div class="container">
      <PaiProps/>

      <hr>

      <PaiEventUnilateral/>

      <hr>

      <PaiEventBidirecional/>
    </div>

  </div>
</template>

<script>
import PaiProps from './components/props/Pai'
import PaiEventUnilateral from './components/evento-unilateral/Pai'
import PaiEventBidirecional from './components/evento-bidirecional/Pai'

export default {
  components: { PaiProps, PaiEventUnilateral, PaiEventBidirecional }
}
</script>

<style scoped>
.lembreteFluxo {
  text-align: center;
  margin-top: 100px;
}

.container {
  text-align: center;
  margin-top: 50px;
}
</style>
