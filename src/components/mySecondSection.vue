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
                                <h4>{{ dataSecondSection.minititle }}</h4>
                                <h2><span>{{ dataSecondSection.prefixtitle }}</span> {{ dataSecondSection.title }}</h2>
                                <p>{{ dataSecondSection.text }}</p>
                            </div>

                            <div class="insidecard-bot">

                                <div class="secarg" v-for="(element,index) in dataSecondSection.insideCard" :key="index">
                                    <span>   <font-awesome-icon :icon="[element.prefixIcon, element.icon]" /></span> <h5>{{ element.title }}</h5>
                                     
                                    <p>{{ element.text }}</p>
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
    height: 40%;
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
</style>
