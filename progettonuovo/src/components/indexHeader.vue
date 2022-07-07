<template>

  <div class="container">
  <!--  implementazione header utilizzando nav-bar importata da bootstrap-->
    <nav class="navbar navbar-expand-lg">
      <div class="container-fluid">
        <img class="img" src="../assets/natura.jpg" alt="">
        <div class="collapse navbar-collapse" id="navbarText">
              <h4><span class="fw-bold">Nature</span> Agency</h4>
        </div>
              <button class="navbar-toggler" style="color:gray" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <i class="fas fa-align-justify"></i>
              </button>
        <div class="collapse navbar-collapse " id="navbarSupportedContent">
              <ul class="navbar-nav ms-auto mx-3 mb-3 mb-lg-0 ">
                  <li class="nav-item mx-2">
                      <a class="nav-link" href="#">Who we are</a>
                  </li>
                  <li class="nav-item mx-2">
                    <a class="nav-link" href="#">Services</a>
                  </li>
                  <li class="nav-item mx-2">
                    <a class="nav-link" href="#">Products</a>
                  </li>
                  <li class="nav-item mx-2">
                    <a class="nav-link" href="#">Blog</a>
                  </li>
                  <li class="nav-item mx-2">
                      <a class="nav-link text-dark" aria-current="page" href="#"><i class="fas fa-search"></i></a>
                  </li>
                  <li class="nav-item mx-2">
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
  name: 'indexHeader',
  
}
</script>


<style scoped lang="scss">
.navbar-toggler {
  color: gray;
  background-color: rgb(194, 184, 184);
}
.img{
  width: 60px
}

.btn:hover{
  background-color: black;
}

ul li a{
  color: black;
}
</style>
