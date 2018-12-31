<template>
  <div class="home">

    <section class="hero is-primary is-bold is-fullheight-with-navbar">
    <!-- Hero head: will stick at the top -->
    <div class="hero-head">
      <nav class="navbar">
        <div class="container">
          <div class="navbar-brand">
            <a class="navbar-item">
              <img src="https://bulma.io/images/bulma-type-white.png" alt="Logo">
            </a>
            <span class="navbar-burger burger" data-target="navbarMenuHeroA">
              <span></span>
              <span></span>
              <span></span>
            </span>
          </div>
          <div id="navbarMenuHeroA" class="navbar-menu">
            <div class="navbar-end">
              <a class="navbar-item is-active">
                Home
              </a>
              <a class="navbar-item">
                About
              </a>
              <a class="navbar-item">
                Portfolio
              </a>
              <span class="navbar-item">
                <a class="button is-primary is-inverted">
                  <span class="icon">
                    <i class="fab fa-github"></i>
                  </span>
                  <span>Download</span>
                </a>
              </span>
            </div>
          </div>
        </div>
      </nav>
    </div>

    <!-- Hero content: will be in the middle -->
    <div class="hero-body columns">
      <div class="column is-one-third">
        <figure class="image is-128x128">
          <img class="is-rounded" src="https://bulma.io/images/placeholders/128x128.png">
        </figure>        
        <h1 class="title">
          Ricky Colson III
        </h1>
        <h2 class="subtitle">
          Designer & Visual Artist
        </h2>
      </div>

     <div class="columns"> 
        <div class="">
          <figure class="image is-4by5">
            <img src="https://bulma.io/images/placeholders/480x600.png">
          </figure>
          <p class="title has-text-dark">My Humble Existence</p>
        </div>         
        <div class="tile box">
          <p class="title has-text-dark">Zooettes</p>
        </div>         
        <div class="tile box">
          <p class="title has-text-dark">Welcome to Autumn</p>
        </div>         
        <div class="tile box">
          <p class="title has-text-dark">Cabells</p>
        </div> 
    </div>        
    </div>   

		<!-- Footer -->
			<footer id="hero-foot">
				<div class="content has-text-centered">
          <p>
            Copyright 2019 Ricky Colson
          </p>
				</div>
			</footer>

    </section>

  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld
  }
}
</script>


