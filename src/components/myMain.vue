<template>
    <main>
        <MyFirstSection :dataFirstSection="this.dataFirstSection"/>
    </main>
</template>


<script>
import MyFirstSection from "./myFirstSection.vue";

export default {
    name: 'myMain',
    components: {
        MyFirstSection,
    },
    data(){
      return {
        dataFirstSection: {
            allTitle: [
                {
                    icon: "fa-user-group",
                    title: 'Human Capital',
                    text: 'Humanizing business: Harness the power of technology to improve the way people work.'
                },
                {
                    icon: "fa-chart-pie",
                    title: 'Core Business ',
                    text: 'It takes innovation approaches to transform, modernize, and run existing platforms.'
                },
                {
                    icon: "fa-gauge-high",
                    title: 'Performance ',
                    text: 'Achieving maximum impact and value from investments in finance and supply chain.'
                },
            ],
            }
        }
        }
    }

</script>


<style>
</style>