<template>
    <header>
        <div class="header-top">
            <div class="container">

                <div class="row align-items-center">

                    <div class="col-5 offset-1"> <i class="fa-solid fa-clock"></i> {{ dataHeader.hours }}</div>
                    <div class="col">
                        <div class="telnumb"> <i class="fa-solid fa-phone"></i> {{ dataHeader.telephone }}</div>
                    </div>
                    <div class="col"> <i class="fa-solid fa-envelope"></i> {{ dataHeader.mail }}</div>
                    <div class="col-2">
                        <!-- Promemoria: Dovrai eseguire ciclo for per ottenere le icone -->
                        <div class="iconbox d-flex">
                            <div class="icon">
                                <i class="fa-brands fa-facebook-f"></i>
                            </div>

                            <div class="icon">
                                <i class="fa-brands fa-twitter"></i>
                            </div>

                            <div class="icon">
                                <i class="fa-brands fa-linkedin-in"></i>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>

        <div class="header-bottom">
            <div class="header-shade">
                <!-- Top Side -->
                <div class="container">
                    <div class="top">
                        <div class="row d-flex">
                            <div class="col-4 offset-1">
                                <div class="mylogo">
                                    <span class="halflogo">NEX</span>GEN
                                </div>
                            </div>
                            <div class="col" v-for="(element, index) in dataHeader.allNav" :key="index">
                                <a class="links" href="#"> {{ element.nav }}</a>
                            </div>

                        </div>
                    </div>
                    <!-- Center side  -->
                    <div class="bottom d-flex justify-content-center">
                        <div class="row ">
                            <div class="col">
                                <div class="title"> LEAD &#126; <span class="halftitle"> Customer</span></div>

                            </div>
                        </div>
                        <div class="row">
                            <div class="col">
                                <div class="subtext">{{ dataHeader.subtext }}</div>

                            </div>
                        </div>
                        <div class="row">
                            <div class="col">
                                <div class="boxbutton subtext">
                                    <div class="btn btn-outline-success mpdi ">   <a href="#">  Get in Touch</a></div>
                                    <div class="btn btn-outline-success mpdi">   <a href="#">  Get in Touch</a></div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>


            </div>

        </div>
    </header>
</template>


<script>

export default {
    name: 'myHeader',
    props: {
        dataHeader: Object
    }

}
</script>

<style scoped lang="scss">
.top {
    height: 40%;
}

.header-top {
    .row {
        height: 100%;
    }
}

.container {
    width: 80%;
}


.icon {
    padding-inline: 0.6rem;
    font-size: 0.7rem;
}

header {
    color: white
}

.header-bottom {
    background-image: url(../assets/images/hero-image.png);
    background-size: cover;
    height: 600px;
    background-position-x: center;
    background-position-y: bottom;

    .row {
        padding-top: 1.2rem;
    }

    .header-shade {
        background-color: rgba(0, 0, 0, 0.7);
        height: 100%;
    }
}

.mylogo {
    letter-spacing: 3px;

    .halflogo {
        border-radius: 13px 1px 1px 13px;
        padding: 8px;
        color: rgba(57, 196, 198);
        background-color: rgba(3, 132, 131, 0.4);
        padding-left: 20px;
    }
}

.title {
    text-align: center;
    font-size: 3rem;
    font-weight: bold;
}

.subtext {
    text-align: center;
    width: 60%;
    margin: 0 auto;
}

.boxbutton {
    padding-inline: 0.5rem;
}

.halftitle {
    padding: 10px;
    background-color: rgba(3, 132, 131, 0.2);
}

.bottom {
    flex-direction: column;
}

.links {
    text-decoration: none;
    color: white;
}

.mpdi {
    margin-inline: 1.5rem;
}
</style>