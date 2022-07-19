<template>
    <!-- Quinta sezione -->
    <section class="quintasection">
        <div class="container-fluid">
            <div class="row">
                <div class="col pdbl">
                    <div class="title">
                        <h4 class="pco"> {{ dataQuintaSection.minititle }} </h4>
                        <h2> {{ dataQuintaSection.title }} <span class="halftitle">{{
                                dataQuintaSection.prefixtitle
                        }}</span></h2>
                    </div>

                    <div class="d-flex">
                        <p class="mywidth60 fsize"> {{ dataQuintaSection.text }} </p>
                        <div class="d-flex rightside">
                            <button> {{ dataQuintaSection.buttonText }}</button>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row">
                <!-- Colonna -->


                <div class="col-4" v-for="(element, index) in dataQuintaSection.allText" :key="index">
                    <!-- Box di una Carta Generata -->
                    <div class="boxcard">
                        <!-- Carta generata -->
                        <div class="mycard">
                            <!-- Icone generate -->
                            <img :src="element.img" :alt="element.alt">
                            <div class="shader"> </div>
                            <p class="">{{ element.text }}</p>
                        </div>
                    </div>
                </div>




            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'myFifthSection',
    props: {
        dataQuintaSection: Object
    }
}
</script>

<style lang="scss" scoped>
.pdbl {
    padding-block: 30px;
}

.container-fluid {
    width: 80%;
}

.thirdsection {
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
        position: relative;
        margin-block: 30px;

        img {
            width: 100%;
            display: block;
        }

        p {
            position: absolute;
            top: 75%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 50%;
            color: white;
            font-weight: bold;
            text-align: center;
            z-index: 99;
        }
    }
}

.halftitle {
    color: rgba(3, 132, 131);
}

.mywidth60 {
    width: 66%;
}

.rightside {
    width: 36%;
    display: flex;
    justify-content: flex-end;
}

.title {
    h4 {
        color: rgba(3, 132, 131);
        font-size: 0.8rem;
        font-weight: bold;
    }
}

.pco {
    font-size: 2rem;
    padding-bottom: 1rem;
}

.fsize {
    font-size: 1rem;
    color: #a2adae;
}

.shader {
    width: 100%;
    height: 100%;
    position: absolute;
    z-index: 99;
    top: 0%;
    left: 0%;
    background-color: rgba(0, 0, 0, 0.5);
}

h2{
    font-weight: bold;
    font-size: 3rem;
}
</style>