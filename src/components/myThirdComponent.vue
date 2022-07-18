<!-- Not per dopo: 
    Stringere width per comparare con altre sezioni , succesivamente mettere una row superiore
     dove aggiungere testo da stampare
 -->

<template>
          <!-- Prima sezione -->
    <section class="thirdsection">
        <div class="container-fluid">
            <div class="row offset-1">
                <!-- Colonna -->


                <div class="col-3">
                    <!-- Box di una Carta Generata -->
                    <div class="boxcard">
                        <!-- Carta generata -->
                        <div class="mycard">
                            <!-- Icone generate -->
                            <div class="icons">
                                <div class="icon">
                                   icona
                                </div>
                            </div>
                            <h2> eee</h2>
                            <p>eee</p>
                        </div>
                    </div>
                </div>

                     <div class="col-3">
                    <!-- Box di una Carta Generata -->
                    <div class="boxcard">
                        <!-- Carta generata -->
                        <div class="mycard">
                            <!-- Icone generate -->
                            <div class="icons">
                                <div class="icon">
                                   icona
                                </div>
                            </div>
                            <h2> eee</h2>
                            <p>eee</p>
                        </div>
                    </div>
                </div>


                     <div class="col-3">
                    <!-- Box di una Carta Generata -->
                    <div class="boxcard">
                        <!-- Carta generata -->
                        <div class="card">
                            <!-- Icone generate -->
                            <div class="icons">
                                <div class="icon">
                                   icona
                                </div>
                            </div>
                            <h2> titolo </h2>
                            <p> contenuto</p>
                            <button>bottone</button>
                        </div>
                    </div>
                </div>


            </div>
        </div>
    </section>
</template>

<script>
export default { 
    name: 'myThirdComponent'
}
</script>

<style lang="scss" scoped>
.thirdsection{
    background-color: lightcoral;
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