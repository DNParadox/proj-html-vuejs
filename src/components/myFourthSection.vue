<template>
          <!-- Quarta sezione -->
    <section class="fourthsection">
        <div class="container-fluid">
            <div class="row">
                <div class="col pdbl">
                    <div class="title text-align-center">
                        <h4 class="pco"> {{ dataFourthSection.minititle}} </h4>
                        <h2><span class="halftitle pco">{{ dataFourthSection.prefixtitle}}</span> {{ dataFourthSection.title}} </h2>
                    </div>

                    <div class="d-flex justify-content-center">
                        <p class="fsize"> {{dataFourthSection.text }}   </p>
                    </div>
                </div>
            </div>
            <div class="row">
                <!-- Colonna -->


                <div class="col-4" v-for="(element,index) in dataFourthSection.insideCard" :key="index">
                    <!-- Box di una Carta Generata -->
                    <div class="boxcard">
                        <!-- Carta generata -->
                        <div class="mycard">
                            <!-- Icone generate -->
                            <div class="icons">
                                <div class="icon">
                                    <span class="pdl"><font-awesome-icon  class="pco" :icon="[element.prefixIcon, element.icon]"/></span>
                                </div>
                            </div>
                            <div class="inside-card">
                                <h2> {{element.title}} </h2>
                                <div class="price">
                                    <span>{{ element.dollar }}</span> <span class="pco"> {{ element.price}}</span> <span> {{ element.monthly}}</span>
                                </div>
                            </div>
                         
                            <ul >
                                <li class="d-flex" v-for="(insideEl,index ) in element.text" :key="index"> <span class="lwidth">{{ insideEl.li}} </span><span class="pdl rwidth"><font-awesome-icon  class="pco" :icon="[insideEl.prefixIcon, insideEl.icon]"/></span></li>
                            </ul>
                    
                           
                        </div>
                    </div>
                </div>

        


            </div>
        </div>
    </section>
</template>

<script>
export default { 
    name: 'myThirdComponent',
    props: {
        dataFourthSection: Object
    }
}
</script>

<style lang="scss" scoped>
.pdl{
    padding-left: 1rem;
}
.pdbl {
    padding-block: 30px;
}
.container-fluid{
    width: 80%;
}
.fourthsection{
    background-color: #e3e7df;
    padding-block: 80px;
}

.row {
    height: 100%;
}

.col {
    height: 100%;
}

.boxcard {
    height: 100%;

      .mycard {
        margin-block: 30px;
        background-color: white;
        padding-block: 60px;
        padding-inline: 40px;
        border-radius: 10px 10px 10px 10px;
    }
}

.icons {
    display: flex;
    justify-content: center;
}

.mywidth60{
    width: 66%;
}

.rightside{
    width: 36%;
    display: flex;  
    justify-content: flex-end;

}

.title{
    text-align: center;
    h2{
    font-weight: bold;
    font-size: 3rem;
    color: black;
    }


    h4{
    color: rgba(3, 132, 131);
    font-size: 0.8rem;
     font-weight: bold;
    }
}

.pco {
    font-size: 3rem;
    padding-bottom: 1rem;
    text-align: center;
}

.fsize{
    font-size: 1rem;
    color: #a2adae;
    text-align: center;
    width: 60%;
    padding-top: 1.5rem
}

.inside-card {
    text-align: center;
    color: rgba(3, 132, 131);
     h2{
        color: black
     }
}

ul .pco {
    font-size: 1rem;
}

.lwidth{
    font-size: 0.9rem;
    width: 82%;
}
.rwidth{
    width: 18%;
}


</style>