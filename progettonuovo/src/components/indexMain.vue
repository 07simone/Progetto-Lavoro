<template>
<div>
    <!-- sezione categorie con descrizione e immagini realizziate anche in maniera responsive -->
<section id="category">
    <div class="container mt-5">
        <div class="row">
            <div class="col-12 col-md-6  col-lg-6" style="font-size:0.8rem">
                <span class="fw-bold">Category</span>
                <h1 style="color:#218491" >Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat dicta officiis quo quae. Obcaecati soluta maxime quaerat </h1>
                <p id="description" style="color:#6F6F6F" >Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat dicta officiis quo quae. Obcaecati soluta maxime quaerat iste officia suscipit sunt! Accusantium error id nam sunt! Laborum nemo maxime incidunt.</p>
                <button class="btn rounded-pill">Read More</button>
            </div>
            <div class="col-12 col-lg-6 mt-3">
                <img class="img-fluid" src="../assets/Photo.png" alt="">
            </div>
        </div>
    </div>
</section>
<section id="cardWrapper">
    <!-- sezione delle card, anch'essa realizzata anche in maniera responsive con l'hover-->
    <div class="container mt-5">
        <div class="row">
            <div class="col-12">
                <h3 id="title">Latest from the blog</h3>
                <p style="color:#6F6F6F">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Est, pariatur animi illo architecto laudantium voluptates assumenda tempore. Velit nulla quidem voluptatem, sit optio temporibus ipsum sapiente iusto magni eum rem.</p>
            </div>
        </div>
        <div class="row">
            <div class="col-12 col-md-6 col-lg-4 mt-3">
                <div class="card " style="width: 18rem;">
                    <img src="../assets/Mask Group 1.png"  alt="...">
                    <div class="card-body">
                        <h5 class="card-title"> <span id="title">Category</span>  / <span id="date" style="color: #999999">June 2020, 13</span> </h5>
                        <p class="card-text">Lorem ipsum dolor sit amet consectetur adipis</p>
                        <div class="wrapperRow d-flex">
                            <div class="riga1"></div>
                                <span>Read more</span>
                            <div class="riga"></div>
                        </div>
                        
                    </div>
                </div>
            </div>
            <div class="col-12 col-md-6  col-lg-4 mt-3">
                <div class="card " style="width: 18rem;">
                    <img src="../assets/pexels-pixabay-531321.png"  alt="...">
                    <div class="card-body">
                        <h5 class="card-title"><span id="title">Category</span> / <span id="date" style="color: #999999">June 2020, 13</span></h5>
                        <p class="card-text">Lorem ipsum dolor sit amet consectetur adipis</p>
                        <div class="wrapperRow d-flex">
                            <div class="riga1"></div>
                                <span>Read more</span>
                            <div class="riga"></div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-12 col-lg-4 mt-3">
                <div class="card " style="width: 18rem;">
                    <img src="../assets/Schermata 2020-05-22 alle 11.59.13.png" alt="...">
                    <div class="card-body">
                        <h5 class="card-title"><span id="title">Category</span> / <span id="date" style="color: #999999">June 2020, 13</span></h5>
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
    button{
        background-color: #218491;
        color:white;
        &:hover{
            background-color: black;
        }
    }
}
#cardWrapper{
    background-color:rgba(224, 220, 220, 0.986);
    padding: 5rem 0; 
    img{
        height: 170px;
    }
    .riga{
        height: 2px;
        background-color: #218491;
        margin-top: 1rem;
        margin-left: 25px;
        width: 50px;
    }
    .riga1{
            height: 2px;
            background-color: #218491;
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
        color: #218491;
    }
}
.right{
    background-image: url(../assets/neve.jpg);
    background-size: cover;
    background-position: center;
    padding: 20rem 0 5rem;
}
.left{
    background-color: #218491;
    padding: 7rem 2rem 5rem;
    color:white
}

#focus{
    .btn:hover{
        background-color:white;
        color:#218491
    }
}

</style>