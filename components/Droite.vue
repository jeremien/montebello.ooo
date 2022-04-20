<template>
    <div class="droite">
        <div class="news">
            <p>{{info.info}}</p>
        </div>
        <div class="resident">
            <p>Les résident·e·s:<br>
                <a href="http://margauxauria.fr/">Margaux Auria</a><br>
                <a href="https://mathildereynaud.com/">Mathilde Reynaud</a><br>
                <a href="https://merrylbouchereau.com/">Merryl Bouchereau</a><br>
                <a href="https://www.geraldinegrammon.com/">Géraldine Grammon</a><br>
                <a href="http://helenehulak.com/">Hélène Hulak</a><br> 
                <a href="http://www.plusartefact.com/index.html">Yoann Jacquon</a><br> 
                <a href="https://kommet.fr/">KOMMET - lieu d’art contemporain</a><br> 
                <a href="https://melissamariller.com/">Mélissa Mariller</a><br> 
                <a href="https://jeremienuel.fr/">Jérémie Nuel</a><br>
                <a href="https://laurapouppeville.fr/">Laura Pouppeville</a><br> 
                <a href="https://www.etsy.com/fr/shop/FogharStudio">Studio Foghar (Donia Ouertani et Nolwenn Michéa)</a><br>             
                <a href="https://studioganek.com/">Studio Ganek</a><br>
            </p>
        </div>
    </div>
</template>

<script>
import marked from 'marked'
export default {
    name: 'Droite',
    props: {
        info: Object
    },
    // data() {
    //     return {
    //         markdown: null
    //     }
    // },
    computed: {
        markdownToHtml(){
            // console.log(this.info.info)
            return marked(this.info.info)

   },

 }
}
</script>