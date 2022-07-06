<template>
<div>
<section id="category">
    <div class="container mt-5">
        <div class="row">
            <div class="col-6">
                <span>Category</span>
                <h1>Lorem ipsum dolor sit amet,consetetur</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat dicta officiis quo quae. Obcaecati soluta maxime quaerat iste officia suscipit sunt! Accusantium error id nam sunt! Laborum nemo maxime incidunt.</p>
                <button class="btn btn-success rounded-pill">Read More</button>
            </div>
            <div class="col-6">
                <img class="img-fluid" src="../assets/slide04.jpg" alt="">
            </div>
        </div>
    </div>
</section>
<section id="cardWrapper">
    <div class="container mt-5">
        <div class="row">
            <div class="col-8">
                <h3>Latest from the blog</h3>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Est, pariatur animi illo architecto laudantium voluptates assumenda tempore. Velit nulla quidem voluptatem, sit optio temporibus ipsum sapiente iusto magni eum rem.</p>
            </div>
        </div>
        <div class="row">
            <div class="col-4">
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
            <div class="col-4">
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
            <div class="col-4">
                <div class="card " style="width: 18rem;">
                    <img src="../assets/nebbia.jpeg" alt="...">
                    <div class="card-body">
                        <h5 class="card-title"><span id="title">Category</span>/ June 2020, 13</h5>
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
    <div class="container-fluid">
        <div class="row">
            <div class="col-6 right">
                
            </div>
            <div class="col-6 left">
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
        margin-left: 10px;
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
        margin-left: 30px;  
        transition: margin 0.5s ease;
        position: relative;
        
        .riga{
            display: none;
        }
        .riga1{
            display: block;
            position: absolute;
            left: -40px;
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
</style>