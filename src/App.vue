<template>
<html>

<body>
    <div class="my-jumbotron" id="my-jumbotron">
    <nav class="navbar navbar-expand">
        <img src="/picture/logo2.png" width="70px" height="70px" class="navbar-brand p-2"/>
        <ul class="navbar-nav">
        <li class="nav-item">
            <a class="nav-link" href="">Home</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="">About</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="">Shop</a>
        </li>
        </ul>
        <div class="collapse navbar-collapse">
          <ul class="nav navbar-nav ml-auto">
          <li class="nav-item mx-3 ">
              <a class="nav-link" href="" ><b-icon icon="person-fill"></b-icon></a>
          </li>
          <li class="nav-item mx-3">
              <a class="nav-link" href=""><b-icon icon="bucket-fill"></b-icon></a>
          </li>
          </ul>
        </div>
        </nav>



       <!-- banner -->
        <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="3500"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- img-src="https://i.picsum.photos/id/1070/5472/3648.jpg" -->
      <!-- img-src="https://i.picsum.photos/id/1071/3000/1996.jpg" -->
      <!-- img-src="https://i.picsum.photos/id/1072/3872/2592.jpg" -->
      <!-- Text slides with image -->
      <b-carousel-slide img-src="/picture/b2.jpg">
        <div class="container text-center" id="jumbo-text-contain">
            <h4 class="display-4 mt-5" style="font-weight: bold;">Welcome To Ditara !</h4>
            <p class="lead">Belanja Mudah di Ditara</p>
            <button type="button" class="btn" id="jumbotron-btn">SHOP NOW !</button>
        </div>
      </b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide img-src="/picture/b2.jpg">
        <div class="container text-center" id="jumbo-text-contain">
            <h4 class="display-4 mt-5" style="font-weight: bold;">Welcome To Ditara !</h4>
            <p class="lead">Belanja Mudah di Ditara</p>
            <button type="button" class="btn" id="jumbotron-btn">SHOP NOW !</button>
        </div>
      </b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide img-src="/picture/b2.jpg">
        <div class="container text-center" id="jumbo-text-contain">
            <h4 class="display-4 mt-5" style="font-weight: bold;">Welcome To Diatara !</h4>
            <p class="lead">Belanja Mudah di Ditara</p>
            <button type="button" class="btn" id="jumbotron-btn">SHOP NOW !</button>
        </div>
      </b-carousel-slide>
    </b-carousel>
  </div>
    </div>



<div id="category-sect">
    <h4 class="font-weight-bold pt-5 text-center"> Shop By Category </h4>
      <section id="tabs" class="project-tab">
        <div class="container-fluid">
            <div class="row justify-content-center">
                <div class="col-md-12">
                    <b-tabs content-class="mt-3" fill>
                    <b-tab title="Men" active>
                    <ul class="container mt-4">
                          <div class="row">
                        <div v-for="(men, index) in men" :key="index" class="my-3 mr-2 text-center">
                          <div class="product-image">
                            <img :src="/picture/ + filename + index + filetype" class="img-responsive h-100 w-100"/>
                            </div>
                          <div class="product-details">
                            <h6 class="display-6 mt-3">{{ men.name }}</h6>
                            <h6 class="display-6 text-muted">Rp.{{ men.price }}</h6>
                          </div>
                        </div>
                    </div>
                    </ul>
                    </b-tab>
                    <b-tab title="Women">
                      <ul class="container mt-4">
                          <div class="row">
                        <div v-for="(women, index) in women" :key="index" class="my-3 mr-2 text-center">
                          <div class="product-image">
                            <img :src="/picture/ + filenama + index + filetype" class="img-responsive h-100 w-100"/>
                            </div>
                          <div class="product-details">
                            <h6 class="display-6 mt-3">{{ women.name }}</h6>
                            <h6 class="display-6 text-muted">Rp.{{ women.price }}</h6>
                          </div>
                        </div>
                    </div>
                    </ul>
                    </b-tab>
                  </b-tabs>

                    </div>
                </div>
            </div>
            </section>
        </div>
		
  </body>

 <footer class="page-footer blue pt-5 mt-5">
<div class="container-fluid text-center text-md-left">
      <div class="row">
        <div class="col-md-6 mt-md-0 mt-3">
          <p class="text-md-left px-5">Ingin kemudahan dalam proses transaksi. Belanja lah di toko kami. Menjual berbagai macam fashion kekinian. Tentunya dengan model yang terbaru setiap minggunya. SHOP NOW !!!.</p>

        </div>

        <hr class="clearfix w-100 d-md-none pb-3">
        <div class="col-md-3 mb-md-0 mb-3">

          <h5 class="text-uppercase">Layanan Kami</h5>

          <ul class="list-unstyled">
            <li>
              <a href="#!">Link 1</a>
            </li>
            <li>
              <a href="#!">Link 2</a>
            </li>
            <li>
              <a href="#!">Link 3</a>
            </li>
            <li>
              <a href="#!">Link 4</a>
            </li>
          </ul>

        </div>
        <div class="col-md-3 mb-md-0 mb-3">

          <h5 class="text-uppercase">TENTANG KAMi</h5>

          <ul class="list-unstyled">
            <li>
              <a href="#!">Link 1</a>
            </li>
            <li>
              <a href="#!">Link 2</a>
            </li>
            <li>
              <a href="#!">Link 3</a>
            </li>
            <li>
              <a href="#!">Link 4</a>
            </li>
          </ul>

        </div>

      </div>

    </div>

    <div class="footer-copyright text-center py-3 mr-3">© 2020 Copyright: Ditara
    </div>
  </footer>

  </html>
</template>

<script>
import axios from 'axios'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

export default {
    data() {
      return {
        slide: 0,
        filetype:".jpg",
        filename:"men",
        filenama:"women",
        sliding: null,
        men: [],
        women: []
      }
    },
  async created () {
    const baseURI = 'https://my-json-server.typicode.com/ditara/ecommerce/db'
    axios.get(baseURI)
      .then((result) => {
        this.men = result.data.men
        this.women = result.data.women
      })
  }
  }
</script>

<style>

#my-jumbotron {
    background-size: cover;
    overflow: hidden;
}
#jumbo-text-contain {
    color: black;
    min-height: 500px;
    padding: 70px;
}
#jumbotron-btn {
    font-size: 20px;
    border: 3px solid ;
    border-radius: 0;
    transition: 0.3s;
}
#jumbotron-btn:hover {
    color:white ;
    border: 1px solid white;
}
#products-container li{
    list-style-type: none;
    height: 250px;
}
.product-image {
    width: 250px;
    transition: 0.3s ease;
}
.project-tab {
    padding: 10%;
    margin-top: -8%;
}
.project-tab #tabs{
    background: #007b5e;
    color: #eee;
}
.project-tab #tabs h6.section-title{
    color: #eee;
}
.project-tab #tabs .nav-tabs .nav-item.show .nav-link, .nav-tabs .nav-link.active {
    color: #20232a;
    background-color: transparent;
    border-color: transparent transparent #f3f3f3;
    border-bottom: 3px solid !important;
    font-size: 16px;
    font-weight: bold;
}
.project-tab .nav-link {
    border: 1px solid transparent;
    border-top-left-radius: .25rem;
    border-top-right-radius: .25rem;
    color: #acbebe;
    font-size: 16px;
    font-weight: 600;
}
.project-tab .nav-link:hover {
    border: none;
}
.project-tab thead{
    background: #f3f3f3;
    color: #333;
}
.project-tab a{
    text-decoration: none;
    color: #333;
    font-weight: 600;
}
.page-footer {
    color: white;
    background: #20232a;
}
</style>
