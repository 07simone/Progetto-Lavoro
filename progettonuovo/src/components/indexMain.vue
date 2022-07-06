<template>
<div>
    <!-- sezione categorie con descrizione e immagini realizziate anche in maniera responsive -->
<section id="category">
    <div class="container mt-5">
        <div class="row">
            <div class="col-12 col-lg-6">
                <span class="fw-bold">Category</span>
                <h1 style="color:mediumturquoise" >Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat dicta officiis quo quae. Obcaecati soluta maxime quaerat </h1>
                <p id="description" >Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat dicta officiis quo quae. Obcaecati soluta maxime quaerat iste officia suscipit sunt! Accusantium error id nam sunt! Laborum nemo maxime incidunt.</p>
                <button class="btn btn-success rounded-pill">Read More</button>
            </div>
            <div class="col-12 col-lg-6 mt-3">
                <img class="img-fluid" src="../assets/slide04.jpg" alt="">
            </div>
        </div>
    </div>
</section>
<section id="cardWrapper">
    <!-- sezione delle card, anch'essa realizzata anche in maniera responsive con l'hover come da voi richiesto-->
    <div class="container mt-5">
        <div class="row">
            <div class="col-8">
                <h3 id="title">Latest from the blog</h3>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Est, pariatur animi illo architecto laudantium voluptates assumenda tempore. Velit nulla quidem voluptatem, sit optio temporibus ipsum sapiente iusto magni eum rem.</p>
            </div>
        </div>
        <div class="row">
            <div class="col col-lg-4 mt-3">
                <div class="card" style="width: 18rem;">
                    <img src="../assets/strada.jpg"  alt="...">
                    <div class="card-body">
                        <h5 class="card-title"> <span id="title">Category</span>  / June 2020, 13</h5>
                        <p class="card-text">Lorem ipsum dolor sit amet consectetur adipis</p>
                        <div class="wrapperRow d-flex">
                            <div class="riga1"></div>
                                <span>Read more</span>
                            <div class="riga"></div>
                        </div>
                        
                    </div>
                </div>
            </div>
            <div class="col col-lg-4 mt-3">
                <div class="card" style="width: 18rem;">
                    <img src="../assets/roccia.jpeg"  alt="...">
                    <div class="card-body">
                        <h5 class="card-title"><span id="title">Category</span> / June 2020, 13</h5>
                        <p class="card-text">Lorem ipsum dolor sit amet consectetur adipis</p>
                        <div class="wrapperRow d-flex">
                            <div class="riga1"></div>
                                <span>Read more</span>
                            <div class="riga"></div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col col-lg-4 mt-3">
                <div class="card " style="width: 18rem;">
                    <img src="../assets/nebbia.jpeg" alt="...">
                    <div class="card-body">
                        <h5 class="card-title"><span id="title">Category</span> / June 2020, 13</h5>
                        <p class="card-text">Lorem ipsum dolor sit amet consectetur adipis</p>
                        <div class="wrapperRow d-flex">
                            <div class="riga1"></div>
                                <span>Read more</span>
                            <div class="riga"></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
<section id="focus">
    <!--  ultima sezione del main, che vado a rappresentare una semplice immagine accompagnata con una descrizione e un bottone che in hover cambierà colore -->
    <div class="container-fluid">
        <div class="row">
            <div class="col-12 col-lg-6 right"></div>
            <div class="col-12 col-lg-6 left">
                <span>On focus</span>
                <h2>Lorem ipsum dolor sit amet,consetetur</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat dicta officiis quo quae. Obcaecati soluta maxime quaerat iste officia suscipit sunt! Accusantium error id nam sunt! Laborum nemo maxime incidunt.</p>
                <button class="btn btn-dark rounded-pill">Read More</button>
            </div>
        </div>
    </div>
</section>
</div>


</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
#category{
    padding: 5rem;
}
#cardWrapper{
    background-color:rgba(224, 220, 220, 0.986);
    padding: 5rem 0; 
    img{
        height: 170px;
    }
    .riga{
        height: 2px;
        background-color: lightseagreen;
        margin-top: 1rem;
        margin-left: 25px;
        width: 50px;
    }
    .riga1{
            height: 2px;
            background-color: lightseagreen;
            margin-top: 1rem;
            margin-left: 10px;
            width: 50px;
            display: none;
        }
    .wrapperRow:hover{
        cursor: pointer;
        margin-left: 15px;  
        transition: margin 1s ease;
        .riga{
            display: none;
        }
        .riga1{
            display: block;
            
        }
    }
    #title{
        color: rgb(49, 212, 212);
    }
}
.right{
    background-image: url(../assets/neve.jpg);
    background-size: cover;
    background-position: center;
    padding: 20rem 0 5rem;
}
.left{
    background-color: aqua;
    padding: 7rem 2rem 5rem;
}
button:hover{
    cursor: pointer;
    transition: background-color 0.5s ease;
    background-color: white;
    color:black
}
</style>