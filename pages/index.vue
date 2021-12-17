<template>
  <div class="container">
    <Gauche />
    <Droite :info="{info}" />
  </div>
</template>

<script>
import Axios from 'axios'
import Gauche from '@/components/Gauche'
import Droite from '@/components/Droite'

export default {
  name: 'IndexPage',
  components: {
    Gauche,
    Droite
  },
  data () {
    return {
      info: null
    }
  },
  mounted () {
    Axios
      .get('https://openschool.art/pad/p/news.montebello.ooo/export/txt')
      .then( response => {
        return this.info = response.data
      })
      .catch(error => console.log(error))
  }
}
</script>
