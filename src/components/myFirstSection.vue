<template>
    <!-- Prima sezione -->
    <section class="firstsection">
        <div class="container">
            <div class="row">
                <!-- Colonna -->
                <div class="col" v-for="(element, index) in dataFirstSection.allTitle" :key="index">
                    <!-- Box di una Carta Generata -->
                    <div class="boxcard">
                        <!-- Carta generata -->
                        <div class="mycard">

                            <div class="icons">
                                <div class="icon">
                                    <font-awesome-icon :icon="['fas', element.icon]" />
                                </div>
                            </div>

                            <h2> {{ element.title }}</h2>
                            <p>{{ element.text }}</p>
                        </div>
                    </div>
                </div>


            </div>
        </div>
    </section>
</template>


<script>
export default {
    name: 'myFirstSection',
    props: {
        dataFirstSection: Object,

    }
}
</script>


<style scoped lang="scss">
.firstsection {
    height: 400px;
    background-color: #e3e7df;
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
        background-color: white;
        padding-block: 60px;
        padding-inline: 40px;
        border-radius: 10px 10px 10px 10px;
    }
}

.icons {
    padding: 10px;
    background-color: #daeced;
    width: 14%;
    border-radius: 50%;
    display: flex;
    justify-content: center;
}
</style>