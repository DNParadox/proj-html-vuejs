<template>
          <!-- Terza sezione -->
    <section class="thirdsection">
        <div class="container-fluid">
            <div class="row">
                <div class="col pdbl">
                    <div class="title">
                        <h4 class="pco"> {{ dataThirdSection.minititle}} </h4>
                        <h2> {{ dataThirdSection.title}} <span class="halftitle">{{ dataThirdSection.prefixtitle}}</span></h2>
                    </div>

                    <div class="d-flex">
                        <p class="mywidth60 fsize"> {{dataThirdSection.text }}   </p>
                        <div class="d-flex rightside">
                             <button> {{ dataThirdSection.buttonText }}</button>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row">
                <!-- Colonna -->


                <div class="col-4" v-for="(element,index) in dataThirdSection.insideCard" :key="index">
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
                            <h2> {{ element.title }}</h2>
                            <p class="fsize">{{ element.text }}</p>
                            <button> {{ dataThirdSection.ButtonText2 }}</button>
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
        dataThirdSection: Object
    }
}
</script>

<style lang="scss" scoped>

.pdbl {
    padding-block: 30px;
}
.container-fluid{
    width: 80%;
}
.thirdsection{
    background-color: #121117;
    padding-block: 80px;
}

.row {
    height: 100%;
}

.col {
    height: 100%;
}

.boxcard {
    display: flex;
    align-items: center;
    height: 100%;

      .mycard {
        margin-block: 30px;
        background-color: #1e2223;
        padding-block: 60px;
        padding-inline: 40px;
        border-radius: 10px 10px 10px 10px;
        h2{
            color:white;
        }
    }
}

.icons {
    width: 14%;
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
    color:white;
    h4{
    color: rgba(3, 132, 131);
    font-size: 0.8rem;
    }
}

.pco {
    font-size: 2rem;
    padding-bottom: 1rem;
}

.fsize{
    font-size: 1rem;
    color: #a2adae;
}
</style>