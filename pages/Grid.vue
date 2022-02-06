<template>
  <div id="app">
        <imageHeader></imageHeader>
        <main>
        <div class="row">
            <div class="col-md-12">
                <div class="body-container">
                    <h2 class="display-4">DRINK MENU</h2>
                    <p class="lead">
                        FIRST STEP: PICK YOUR FAVORITE DRINK! </p>
                    <div class="container">
                        <div class="row">
                            <div class="col">
                                <div class="card">
                                    <img class="card-img-top" src="../static/img/BLACK.png" alt="CBlack Milk Tea">
                                    <div class="card-body">
                                        <h4 class="card-title">Black Milk Tean</h4>
                                        <p class="card-text">
                                            紅茶拿鐵
                                        </p>
                                        <a href="#!" class="btn btn-primary">ADD!</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col">
                                <div class="card">
                                    <img class="card-img-top" src="../static/img/PASSION.png" alt="Passion Fruit Tea">
                                    <div class="card-body">
                                        <h4 class="card-title">Passion Fruit Tea</h4>
                                        <p class="card-text">
                                            百香綠茶
                                        </p>
                                        <a href="#!" class="btn btn-primary">ADD!</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col">
                                <div class="card">
                                    <img class="card-img-top" src="../static/img/GRAPE.png" alt="Grapefruit Green Tea">
                                    <div class="card-body">
                                        <h4 class="card-title">Grapefruit Green Tea</h4>
                                        <p class="card-text">
                                            葡萄柚綠茶
                                        </p>
                                        <a href="#!" class="btn btn-primary">ADD!</a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="container">
                        <div class="row">
                            <div class="col">
                                <div class="card">
                                    <img class="card-img-top" src="../static/img/taro.jpeg" alt="Taro Milk Tea">
                                    <div class="card-body">
                                        <h4 class="card-title">Taro Milk Tea</h4>
                                        <p class="card-text">
                                            芋頭鮮奶
                                        </p>
                                        <a href="#!" class="btn btn-primary">ADD!</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col">
                                <div class="card">
                                    <img class="card-img-top" src="../static/img/lemon.jpeg" alt="Lemon Black Tea">
                                    <div class="card-body">
                                        <h4 class="card-title">Lemon Black Tea</h4>
                                        <p class="card-text">
                                            檸檬紅茶
                                        </p>
                                        <a href="#!" class="btn btn-primary">ADD!</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col">
                                <div class="card">
                                    <img class="card-img-top" src="../static/img/brown.jpeg" alt="Brown Sugar Milk Tea">
                                    <div class="card-body">
                                        <h4 class="card-title">Brown Sugar Milk Tea</h4>
                                        <p class="card-text">
                                            黑糖鮮奶茶
                                        </p>
                                        <a href="#!" class="btn btn-primary">ADD!</a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>
    <footerNormal></footerNormal>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
import imageHeader from '../components/imageHeader.vue'
import footerNormal from '../components/footerNormal.vue'

export default {
  name: 'Grid',
  components: {
      imageHeader,
      footerNormal

  }
}
</script>

<style>
.body-container {
    margin: 1em;
    margin-right: 10em;
    margin-left: 10em;
    text-align: center;
}
.top-menu {
    display: flex;
    flex-direction: row;
    justify-content: center;
}

.nuxt-link {
  padding: 1em;
}
.button {
    background-color: #4CAF50; /* Green */
    border: none;
    color: white;
    padding: 15px 32px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin: .5em;
    cursor: pointer;
  }

@media only screen and (min-width: 0px) {
    .body-container {
        margin: 0em;
        margin-right: 0em;
        margin-left: 0em;
        text-align: center;
    }

}

@media only screen and (min-width: 768px) {
    .body-container {
        margin: 1em;
        margin-right: 15em;
        margin-left: 15em;
        text-align: center;
    }
}

@media only screen and (min-width: 2000px) {
    .body-container {
        margin: 1em;
        margin-right: 40em;
        margin-left: 40em;
        text-align: center;
    }
}

.jumbotron {
    background-image: url("../static/img/blossoms.jpg");
    background-size: cover;
    display: flex;
    flex-direction: column;
    text-align: center;
}

.header-container {
    margin: 1em;

}
.top-menu {
    display: flex;
    flex-direction: row;
    justify-content: center;
}
.footer-container {
    padding: 5em;
    background-color: rgb(59, 42, 133);
}




</style>
