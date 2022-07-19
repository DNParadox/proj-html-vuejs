<template>
    <section class="settimasection">
               <div class="container-fluid">
            <div class="row justify-content-evenly">
                <div class="col offset-3 d-flex">
                    <div class="center d-flex">
                      <div class="myCard">
                        <h5 class="minititle"> {{ dataSettimaSection.minititle}}</h5>
                        <h2 class="title"> {{ dataSettimaSection.title }} <span class="halftitle">{{ dataSettimaSection.prefixTitle }}</span></h2>
                        <p class="text"> {{ dataSettimaSection.text }}</p>

                        <div class="inputsection d-flex"> 

                            <input type="text" placeholder="Name">
                            <input type="mail" placeholder="Email">
                            <input type="text" placeholder="Phone">

                         <select name="" id="">
                             <option value="A">More info</option>
                         </select>

                        </div>
                         <textarea rows="4" cols="50" name="comment" form="usrform" placeholder="Message">
                        </textarea>
                           <button> {{dataSettimaSection.button}} </button>
                   
                      </div>
                   
                    </div>
                         
                
                </div>
                <div class="col">
                        <div class="right d-flex">

                        <div class="anothercard">
                            <h2> {{ dataSettimaSection.title2 }}</h2>
                            <p> {{ dataSettimaSection.text2 }}</p>
                            <p> {{ dataSettimaSection.text3 }}</p>
                            <div class="icontext" v-for="(element,index) in dataSettimaSection.AllRight" :key="index">
                                <span class="icon"><font-awesome-icon :icon="['fa-solid', element.icon]" />  </span>
                                <span>{{ element.text }} </span>
                             
                            </div>
                            <button>{{dataSettimaSection.button2}}</button>
                        </div>

                    </div>
                </div>
            </div>

        </div>

    </section>
</template>


<script>
export default {
    name: 'mySettimaSection',
    props: {
        dataSettimaSection: Object
    }
}
</script>

<style scoped lang="scss">
  .settimasection{
    height: 500px;
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
        align-items: center;
        height: 100%;
    }

.minititle{
    font-size:0.8rem;
    font-weight: bold;
    color: rgb(3, 132, 131);
}
.title{
    color:black;
    font-weight:bold;
    font-size: 3rem;
    margin-block: 20px;
}
    .text { 
        font-size: 0.8rem;
        color: #a2adae;
    }
.halftitle{
    color: rgb(3, 132, 131);
}
.inputsection{
    display: flex;
    flex-wrap: wrap;
}

input, select{
    border: none;
    margin-block: 8px;
    background-color: #e3e7df;
    padding-block: 5px;
    padding-left: 10px;
    border-radius: 5px;
    width: 40%;
    margin-right: 12px;
}
button {
    margin-top: 10px;
    display: block;
}

textarea{
    border: none;
    width: 82%;
    border-radius: 5px;
    background-color: #e3e7df;
    padding-left: 10px;
    padding-top: 10px;
    margin-top: 10px;
}

select{
    color: #a2adae;
}

.right{
    height: 100%;
    justify-content: center;
    flex-direction: column;
}

.icon {
    margin-inline: 15px;
}
.icontext{
    color:rgb(3, 132, 131);
    margin-block: 25px;
}
.anothercard{

    p{
        width: 60%;
        color: #a2adae;
    }
}
</style>