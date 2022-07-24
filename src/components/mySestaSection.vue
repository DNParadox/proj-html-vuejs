<template>
    <section class="sestasection">
        <div class="container-fluid">
            <div class="row">
                <div class="col">
                    <div class="center d-flex">
                      <div class="myCard">
                        <h5 class="minititle"> {{ dataSestaSection.minititle}}</h5>
                        <h2 class="title"> <span class="halftitle">{{ dataSestaSection.prefixTitle }}</span>{{ dataSestaSection.title }} </h2>
                        <p class="text"> {{ dataSestaSection.text }}</p>
                      </div>

                      <div class="inputsection d-flex"> 
                        <input type="text" placeholder="Name">
                        <input type="mail" placeholder="Email">
                        <button> {{dataSestaSection.button}}</button>
                      </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>


<script>
export default {
    name: 'mySestaSection',
    props: {
        dataSestaSection: Object
    }
}
</script>
    
<style scoped lang="scss">
    .sestasection{
        background-image: url(../assets/images/bg-1.jpg);
        height: 300px;
        background-size: cover;
        background-position-x: 10%;
        background-position-y: 40%;
    }

.row  {
    height: 100%;
}

.container-fluid{
    height: 100%;
}

.col {
    height: 100%
}
    .center{
        color: red;
        justify-content: center;
        align-items: center;
        height: 100%;
    }
.minititle{
    font-size:0.8rem;
    font-weight: bold;
    color: rgb(3, 132, 131);
}
.title{
    color:white;
    font-weight:bold;
    font-size: 3rem;
    margin-block: 20px;
}
    .text { 
        width: 62%;
        font-size: 0.8rem;
        color: #a2adae;
    }

.inputsection{
    flex-direction: column;
    width: 20%;
}

input{
    border: none;
    margin-block: 8px;
    background-color: rgba(255,255,255, 0.3);
    padding-block: 5px;
    padding-left: 10px;
    width: 150%;
    border-radius: 5px;
}
button {
    margin-top: 10px
}
</style>