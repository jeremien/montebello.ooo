<template>
  <div class="container">
    <Gauche />
    <Droite />
  </div>
</template>

<script>
// import Header from '@/components/Header';
import Gauche from '@/components/Gauche'
import Droite from '@/components/Droite'

export default {
  name: 'IndexPage',
  components: {
    Gauche,
    Droite
  }
}
</script>
