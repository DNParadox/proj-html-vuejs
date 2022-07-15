<template>
    <header>
        <div class="header-top">
            <div class="container mx-auto">

                <div class="row justify-content-evenly mycontainer align-items-center">

                    <div class="col-4 off-set-xl-1"> Open Hours: Mon-Sat - 9:00 - 18:00</div>
                    <div class="col-2">
                        <div class="telnumb">+1 (222) 222 333 4444</div>
                    </div>
                    <div class="col-1"> m96francesco@gmail.com</div>
                    <div class="col-1 off-set-xl-1">
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
           <div class="container"> header bottom</div>
        </div>
    </header>
</template>


<script>
export default {
    name: 'myHeader'
}
</script>

<style>
.container {
    height: 100%;
    width: 80%;
}

.row {
    height: 100%;
}

.icon {
    padding-inline: 0.2rem;
}

.header-bottom {
    background-image: url();
}
</style>