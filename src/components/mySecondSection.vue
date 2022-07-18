<template>
    <section class="secondsection">
        <div class="d-flex">
            <!-- Sezione divisa in due parti uguali con una width al 50% -->
            <div class="mywidth">
                <div class="row">
                    <div class="col-6 offset-5">
                        <!-- Carta che verrà divisa in due parti, top-bottom -->
                      <div class="mycard d-flex justify-content-center">
                           <div class="insidecard-top">
                                <h4 class="smalltitle">{{ dataSecondSection.minititle }}</h4>
                                <h2 class="title"><span class="halftitle">{{ dataSecondSection.prefixtitle }}</span> {{ dataSecondSection.title }}</h2>
                                <p class="text">{{ dataSecondSection.text }}</p>
                            </div>

                            <div class="insidecard-bot">

                                <div class="secarg" v-for="(element,index) in dataSecondSection.insideCard" :key="index">
                                    <span class="pdl"><font-awesome-icon  class="test" :icon="[element.prefixIcon, element.icon]"/></span>
                                    <h5 class="title">{{ element.title }}</h5> 
                                    <p class="text">{{ element.text }}</p>
                                </div>

                            </div>  
                      </div>
                    </div>
                </div>
            </div>
            <!-- Right Side . IMG  rinominare ALT in seguito-->

            <div class="mywidth">
                <img :src="dataSecondSection.img" :alt="dataSecondSection.alt">
            </div>

        </div>

    </section>


</template>

<script>
export default {
    name: 'mySecondSection',
    props: {
        dataSecondSection: Object
    }
}
</script>


<style scoped lang="scss">
/* Regola generale di questa sezione. Divisa in due blocchi sx/dx a 50% */
.mywidth {
    width: 50%;
    img {
        width: 100%;  
        height: 600px;
        object-fit: contain;
        object-position: right;
    }
}
.mycard{
    height: 600px;
    align-items: center;
    flex-direction: column;
}
.insidecard-top{
    height: 30%;
}
.insidecard-bot{
    height: 30%;
    display: flex;
    flex-wrap: wrap;
}

.secarg{
    width: calc(100% / 2);
    flex-wrap: wrap;
    display: flex;
}

.smalltitle {
    font-size: 12px;
    font-weight: bold;
    color: rgba(3, 132, 131);
    padding-bottom: 10px;
}

.halftitle{
    color: rgba(3, 132, 131);
    background-color: rgba(3, 132, 131, 0.2);
    padding-block: 5px;
    padding-inline: 15px;
}

.title{
    font-weight: bold;
}

.text{
    font-size: 0.8rem;
    color: #a2adae;
}

.pdl {
    padding-inline: 5px;
}
.test {
   color: rgba(3, 132, 131);
}
</style>
