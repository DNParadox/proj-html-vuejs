<template>
    <header>
        <div class="header-top">
            <div class="container">

                <div class="row align-items-center">

                    <div class="col-4 offset-2"> Open Hours: Mon-Sat - 9:00 - 18:00</div>
                    <div class="col">
                        <div class="telnumb">+1 (222) 222 333 4444</div>
                    </div>
                    <div class="col"> m96francesco@gmail.com</div>
                    <div class="col-2">
                        <!-- Promemoria: Dovrai eseguire ciclo for per ottenere le icone -->
                        <div class="iconbox d-flex">
                            <div class="icon">
                                icon
                            </div>

                            <div class="icon">
                                icon
                            </div>

                            <div class="icon">
                                icon
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>

        <div class="header-bottom">
            <div class="header-shade">
                <div class="container">
                    <div class="row">
                        <div class="col-3 offset-2">
                            <div class="mylogo">
                                <span class="halflogo">NEX</span>GEN </div>
                            </div>
                        <div class="col"> <a href="#"> Test</a> </div>
                        <div class="col">test</div>
                        <div class="col">test</div>
                        <div class="col">test</div>
                        <div class="col">test</div>
                        <div class="col">test</div>
                        <div class="col">test</div>
                    </div>
                </div>
            </div>

        </div>
    </header>
</template>


<script>
export default {
    name: 'myHeader'
}
</script>

<style lang="scss">
.container {
    height: 100%;
    width: 80%;
}
.header-bottom {
    .row {
    height: 100%;
    padding-top: 1.2rem;
    }
}

.icon {
    padding-inline: 0.2rem;
}

header {
    color: white
}

.header-bottom {
    background-image: url(../assets/images/hero-image.png);
    background-size: cover;
    height: 500px;
    background-position-x: center;
    background-position-y: bottom;

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
</style>