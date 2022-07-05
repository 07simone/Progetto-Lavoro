<template>
  <div class="container">
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container-fluid">
        <img class="img" src="../assets/nature.jpg" alt="">
        <div class="collapse navbar-collapse" id="navbarText">
              <h4>Nature Agency</h4>
        </div>
        <div class="collapse navbar-collapse " id="navbarSupportedContent">
              <ul class="navbar-nav ms-auto mx-3 mb-3 mb-lg-0 ">
                  <li class="nav-item">
                      <a class="nav-link" href="#">Who we are</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link" href="#">Services</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link" href="#">Products</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link" href="#">Blog</a>
                  </li>
                  <li class="nav-item">
                      <a class="nav-link text-dark" aria-current="page" href="#"><i class="fas fa-search"></i></a>
                  </li>
                  <li class="nav-item">
                      <button type="button" class="btn btn-success rounded-pill">Contact Us</button>
                  </li>
              </ul>
            </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  
}
</script>


<style scoped lang="scss">
.img{
  width: 60px
}
</style>
