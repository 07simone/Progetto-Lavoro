<template>

    <div>
    <!--  realizzazione di un carosello di immagini con vuejs e scss, utilizzando i props e le funzione per lo scorrimento delle immagini -->
        <div class="carousel-inner text-center">
            <div v-for="(item, index) in items" :key="index" class="carousel-item" :class="{ active: currentSlide == index }">
                <img class="d-block w-100" :src="item.img" />
                <div class="container">
                    <div class="carousel-caption text-start">
                        <h6>{{ item.title }}</h6>
                        <h1>{{item.subtitle}}</h1>
                        <p class="d-none d-md-block">{{ item.caption }}</p>
                        <button type="button" class="btn rounded-pill">Read more</button>
                    </div>
                </div>
            </div>
            <span class="carousel-control-prev" role="button" @click="prevSlide">
                <i class="fas fa-angle-left"></i>
                <span class="sr-only">Previous</span>
            </span>
            <span class="carousel-control-next" role="button" @click="nextSlide">
                <i class="fas fa-angle-right"></i>
                <span class="sr-only">Next</span>
            </span>
        </div>
    </div>


</template>

<script>
export default {
name: "IndexJumbotron",
props: ["items"],
data() {
    return {
    currentSlide: 0,
    timerId: null,
    };
},

methods: {
    isCurrent(value) {
    return this.currentSlide == value;
    },
    setCurrent(value) {
    this.currentSlide = value;
    },
    nextSlide() {
    this.currentSlide =
        this.currentSlide < this.items.length - 1 ? this.currentSlide + 1 : 0;
    },
    prevSlide() {
    this.currentSlide =
        this.currentSlide > 0 ? this.currentSlide - 1 : this.items.length - 1;
    },
    
},

};


</script>

<style lang="scss" scoped>
button{
    background-color: #218491;
    color: white;
}
    button:hover{
        background-color: white;
        color: black;
    }

.carousel-control-prev i,
.carousel-control-next i {
  color: white;
  font-size: 3rem;
}
  .carousel-caption {
    z-index: 1;
  }
</style>