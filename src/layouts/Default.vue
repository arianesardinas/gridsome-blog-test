<template>
  <div class="container">
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Navbar</a>
      <button
          class="navbar-toggler"
          type="button"
          data-mdb-toggle="collapse"
          data-mdb-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
      >
        <i class="fas fa-bars"></i>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav justify-content-center">
          <li class="nav-item">
            <g-link class="nav-link active" to="/">Home</g-link>


          </li>
          <li class="nav-item">
            <g-link class="nav-link " to="/about/">About</g-link>

          </li>


        </ul>
      </div>
    </div>

  </nav>

  <slot/>
    <div class="container">
    <footer class="pt-4 my-md-5 pt-md-5 border-top">
      <div class="row">
        <div class="col-12 ">
          <p class=" justify-content-center">  Praeterea iter est quasdam res quas ex communi.</p>

        </div>
      </div>
      <div class="row">

        <div class="col-6 col-md">
          <h5>Features</h5>
          <ul class="list-unstyled text-small">
            <li><a class="text-muted" href="#">Cool stuff</a></li>

          </ul>
        </div>
        <div class="col-6 col-md">
          <h5>Resources</h5>
          <ul class="list-unstyled text-small">
            <li><a class="text-muted" href="#">Resource</a></li>

          </ul>
        </div>
        <div class="col-6 col-md">
          <h5>About</h5>
          <ul class="list-unstyled text-small">
            <li><a class="text-muted" href="#">Team</a></li>

          </ul>
        </div>
      </div>
    </footer>
  </div>
  </div>

</template>
<script>
import BootstrapVue from 'bootstrap-vue'
import {BButton} from 'bootstrap-vue'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'


export default {
  components: {
    BootstrapVue,
    BButton
  }

}

</script>


<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>
body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  margin:0;
  padding:0;
  line-height: 1.5;
}

.layout {
  max-width: 760px;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
}

.nav__link {
  margin-left: 20px;
}
</style>
