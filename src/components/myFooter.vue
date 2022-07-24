<template>
    <footer>
        <div class="container">
            <div class="myContainer">
                <div class="row">

                    <div class="col">
                        <ul class="ulflex">
                            <li class="title wth"> <span class="halflogo">{{ dataFooter.preFixLogo }}</span> <span class="logo">
                                {{ dataFooter.logo }}</span> 
                            </li>
                            <li class="text"> {{ dataFooter.text }}</li>
                            <li class="data">
                                <font-awesome-icon :icon="['fa-solid', dataFooter.icon1]" /> {{ dataHeader.telephone }}
                            </li>
                            <li class="data">
                                <font-awesome-icon :icon="['fa-solid', dataFooter.icon2]" /> {{ dataHeader.mail }}
                            </li>
                            <li class="data">
                                <font-awesome-icon :icon="['fa-solid', dataFooter.icon3]" /> {{ dataFooter.location }}
                            </li>
                            <li> <button> <a href="#"> {{ dataFooter.button }}</a></button> </li>
                        </ul>
                    </div>


                    <div class="col">

                        <ul class="ulflex">
                            <div class="card">
                                <li class="title"> {{ dataFooter.title1 }}</li>
                                <li v-for="(element, index) in dataFooter.about" :key="index">
                                    <span class="icons">
                                        <font-awesome-icon :icon="['fa-solid', element.icon]" />
                                    </span>

                                    <span>
                                        <a href="#">{{ element.text }}</a>
                                    </span>
                                </li>
                            </div>
                        </ul>
                    </div>



                    <div class="col">

                        <ul class="ulflex">
                            <div class="card">
                                <li class="title"> {{ dataFooter.title2 }}</li>
                                <li v-for="(element, index) in dataFooter.services" :key="index">
                                    <span class="icons">
                                        <font-awesome-icon :icon="['fa-solid', element.icon]" />
                                    </span>

                                    <span>
                                        <a href="#">{{ element.text }}</a>
                                    </span>
                                </li>
                            </div>
                        </ul>
                    </div>

                    <div class="col">

                        <ul class="ulflex">
                            <div class="card">
                                <li class="title"> {{ dataFooter.title2 }}</li>
                                <li v-for="(element, index) in dataFooter.support" :key="index">
                                    <span class="icons">
                                        <font-awesome-icon :icon="['fa-solid', element.icon]" />
                                    </span>

                                    <span>
                                        <a href="#"> {{ element.text }}</a>
                                    </span>
                                </li>
                            </div>
                        </ul>
                    </div>



                </div>
                <div class="othercontainer d-flex">
                    <p class="footerbottomtext"> {{ dataFooter.footerBottomText }}</p>
                    <p> {{ dataFooter.footerBottomText2 }} <span class="codings"> {{ dataFooter.footerBottomText3}}</span></p>

                </div>
            </div>
        </div>

   
    </footer>
</template>



<script>
export default {
    name: 'myFooter',
    props: {
        dataFooter: Object,
        dataHeader: Object
    }
}
</script>


<style scoped lang="scss">
footer {
    background-color: #121117;
    color: #a2adae;
    height: 600px;
}

a {
    color: #a2adae;
}

.row {
    height: 90%;
}
.col {
    height: 100%;
}

.card {
    background-color: #1e2223;
    border-radius: 13px;
    padding-inline: 2rem;
    padding-block: 1.5rem;
}

.myContainer {
    width: 85%;
    margin: 0 auto;
    height: 100%;
}

.ulflex {
    display: flex;
    flex-direction: column;
    justify-content: center;
    height: 100%;
}

.icons {
    padding-right: 0.5rem;

}

li {
    line-height: 2rem;
}

.title {
    font-weight: bold;
    font-size: 24px;
    color: white;
    padding-bottom: 1rem;
}

.halflogo {
    border-radius: 13px 1px 1px 13px;
    padding: 8px;
    padding-left: 8px;
    color: rgb(57, 196, 198);
    background-color: rgba(3, 132, 131, 0.4);
    padding-left: 20px;
}
.text {
    padding-block: 1rem;
}

.data {
    line-height: 2rem;
}
.wth {
    letter-spacing: 5px;
}

.othercontainer {
    height: 10%;
    justify-content: center;
    align-items: center;
    .footerbottomtext{
        width: 67%;
    }
    .codings{
      color: rgb(3, 132, 131);
    }
}


</style>