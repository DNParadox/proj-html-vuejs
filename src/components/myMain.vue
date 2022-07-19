<template>
    <main>
        <MyFirstSection :dataFirstSection="this.dataFirstSection" />
        <MySecondSection :dataSecondSection="this.dataSecondSection" />
        <MyThirdComponent :dataThirdSection="this.dataThirdSection" />
        <MyFourthSection :dataFourthSection="this.dataFourthSection" />
        <myFifthSection :dataQuintaSection="this.dataQuintaSection" />
    </main>
</template>


<script>
import MyFirstSection from "./myFirstSection.vue";
import MySecondSection from "./mySecondSection.vue";
import MyThirdComponent from "./myThirdComponent.vue";
import MyFourthSection from "./myFourthSection.vue";
import myFifthSection from "./myFifthSection.vue";

export default {
    name: 'myMain',
    components: {
    MyFirstSection,
    MySecondSection,
    MyThirdComponent,
    MyFourthSection,
    myFifthSection
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
            },
            dataFourthSection: {
                minititle: 'MONTLY PLANS',
                title: 'Table',
                prefixtitle: 'Pricing ',
                buttonText: 'SEE ALL',
                ButtonText2: 'READ MORE',
                text: 'We can help you deliver and execute your future, wherever you compete, using the latest technologies, from strategy development to implementation.',
                insideCard: [
                    {
                        prefixIcon: 'fas',
                        icon: 'fa-rocket',
                        title: 'Standard',
                        price: '490',
                        dollar: '$',
                        monthly: '/mo ',
                        text: [
                            {
                                prefixIcon: 'fas',
                                li: 'Standard Accounting',
                                icon: 'fa-check',
                            },
                            {
                                prefixIcon: 'fas',
                                li: 'Platform Access',
                                icon: 'fa-check',
                            },
                            {
                                prefixIcon: 'fas',
                                li: 'Business Orientation',
                                icon: 'fa-x',
                            },
                            {
                                prefixIcon: 'fas',
                                li: 'Dedicated Consultant',
                                icon: 'fa-x',
                            },
                            {
                                prefixIcon: 'fas',
                                li: 'Personal Assistance',
                                icon: 'fa-x',
                            }
                        ],
                    },
                    {
                        prefixIcon: 'fas',
                        icon: 'fa-suitcase',
                        price: '890',
                        dollar: '$',
                        monthly: '/mo ',
                        title: 'Professional',
                        text: [
                            {
                                prefixIcon: 'fas',
                                li: 'Standard Accounting',
                                icon: 'fa-check',
                            },
                            {
                                prefixIcon: 'fas',
                                li: 'Platform Access',
                                icon: 'fa-check',
                            },
                            {
                                prefixIcon: 'fas',
                                li: 'Business Orientation',
                                icon: 'fa-check',
                            },
                            {
                                prefixIcon: 'fas',
                                li: 'Dedicated Consultant',
                                icon: 'fa-x',
                            },
                            {
                                prefixIcon: 'fas',
                                li: 'Personal Assistance',
                                icon: 'fa-x',
                            }
                        ],
                    },
                    {
                        prefixIcon: 'fas',
                        icon: 'fa-gem',
                        price: '1390',
                        dollar: '$',
                        monthly: '/mo ',
                        title: 'Ultimate',
                        text: [
                            {
                                prefixIcon: 'fas',
                                li: 'Standard Accounting',
                                icon: 'fa-check',
                            },
                            {
                                prefixIcon: 'fas',
                                li: 'Platform Access',
                                icon: 'fa-check',
                            },
                            {
                                prefixIcon: 'fas',
                                li: 'Business Orientation',
                                icon: 'fa-check',
                            },
                            {
                                prefixIcon: 'fas',
                                li: 'Dedicated Consultant',
                                icon: 'fa-check',
                            },
                            {
                                prefixIcon: 'fas',
                                li: 'Personal Assistance',
                                icon: 'fa-check',
                            }
                        ],
                    }
                ],
            },
            dataQuintaSection: {
            minititle: 'OUR EDITIORIAL CONTENT',
            title: 'Latest',
            prefixtitle: 'News',
            text: 'Every week we publish content about what is best in the business world.',
            buttonText: 'SEE ALL',
            
            allText: [
                {
                    alt: 'Una disegnatrice',
                    img: require('../assets/images/news-1.jpg'),
                    text: 'Increasing creativity is possibile for everyone'
                },
                {
                    alt: 'palese ad delle Airpods',
                    img: require('../assets/images/news-2.jpg'),
                    text: 'Because market research is part of the business plan'
                },
                {
                    alt: 'Smart Working',
                    img: require('../assets/images/news-3.jpg'),
                    text: 'Working from home is now a trend'
                },

            ]
        }
        }
    }
}

</script>


<style>
</style>