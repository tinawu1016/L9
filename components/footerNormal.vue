<template>
  <div id="footerNormal">
     <footer>
          <div class="row">
              <div class="col-md-12">
                  <div class="footer-container">
                      <div class="top-menu">
                          <ul class="nav">
                              <li class="nav-item">
                                  <nuxt-link to="/" class='nuxt-link'> Home </nuxt-link>
                              </li>
                              <li class="nav-item">
                                  <nuxt-link to="/accordion-questions" class='nuxt-link'> About Us </nuxt-link>
                              </li>
                              <li class="nav-item">
                                  <nuxt-link to="/Grid" class='nuxt-link'> Faculties </nuxt-link>
                              </li>
                              <li class="nav-item">
                                  <nuxt-link to="/Images" class='nuxt-link'> Drink Menu </nuxt-link>
                              </li>
                          </ul>
                      </div>

                  </div>
              </div>
          </div>
      </footer>
  </div>
</template>

<script>
export default {
  name: 'footerNormal'
}
</script>

<style>
.footer-container {
    padding: 5em;
    background-color: rgb(59, 42, 133);
}
.nuxt-link {
  padding: 1em;
}

</style>
