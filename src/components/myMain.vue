<template>
    <main>
        <MyFirstSection :dataFirstSection="this.dataFirstSection" />
        <MySecondSection :dataSecondSection="this.dataSecondSection" />
        <MyThirdComponent :dataThirdSection="this.dataThirdSection" />
    </main>
</template>


<script>
import MyFirstSection from "./myFirstSection.vue";
import MySecondSection from "./mySecondSection.vue";
import MyThirdComponent from "./myThirdComponent.vue";

export default {
    name: 'myMain',
    components: {
        MyFirstSection,
        MySecondSection,
        MyThirdComponent
    },
    data() {
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
            },
            dataSecondSection: {
                minititle: 'About the Network',
                prefixtitle: 'The',
                title: 'Company',
                img: require('../assets/images/about-3.jpg'),
                alt: 'Working in the office',
                text: 'For 12 years we have been providing audit and warranty, financial advice, risk advice, taxes and related services to select clients',
                insideCard: [
                    {
                        // Rivedere questa icona, placeholder ATM
                        prefixIcon: 'fas',
                        icon: 'fa-user',
                        title: 'Tradition',
                        text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. '
                    },
                    {
                        prefixIcon: 'fas',
                        icon: 'fa-lock',
                        title: 'Security',
                        text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. '
                    },
                    {
                        prefixIcon: 'fas',
                        icon: 'fa-pen-to-square',
                        title: 'Certificate',
                        text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. '
                    },
                    {
                        prefixIcon: 'fas',
                        icon: 'fa-helmet-safety',
                        title: 'Expertise',
                        text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. '
                    },
                ]
            },
            dataThirdSection: {
                icon: ' ',
                minititle: 'OUR BUSINESS AREAS',
                title: 'Excellence in ',
                prefixtitle: 'Services',
                buttonText: 'SEE ALL',
                ButtonText2: 'READ MORE',
                text: 'We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowned professionals. These are some options that you can hire', 
                insideCard: [
                    {
                        prefixIcon: 'fas',
                        icon: 'fa-helmet-safety',
                        title: 'Audit & Assurance',
                        text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. '
                    },
                    {
                        prefixIcon: 'fas',
                        icon: 'fa-suitcase',
                        title: 'Financial Advisory',
                        text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. '
                    },
                    {
                        prefixIcon: 'fas',
                        icon: 'fa-chart-simple',
                        title: 'Analytics and M&A',
                        text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. '
                    },
                    {
                        prefixIcon: 'fas',
                        icon: 'fa-plane-departure',
                        title: 'Middle Marketing',
                        text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. '
                    },
                    {
                        prefixIcon: 'fas',
                        icon: 'fa-earth-europe',
                        title: 'Legal Consulting',
                        text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. '
                    },
                    {
                        prefixIcon: 'fas',
                        icon: 'fa-inbox',
                        title: 'Regulatory Risk',
                        text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. '
                    },
                ]
            }
        }
    }
}

</script>


<style>
</style>