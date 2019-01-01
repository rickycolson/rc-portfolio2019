<template>
  <div class="home">

    <section class="hero is-dark is-bold is-fullheight-with-navbar">
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
    <div class="columns container is-fluid">
      <div class="column is-one-quarter">
        <figure class="image is-128x128">
          <img class="is-rounded" src="https://bulma.io/images/placeholders/128x128.png">
        </figure>
        <div class="content has-text-left" style="padding-top: 2em">
          <h1 class="title is-2">
            Ricky Colson III
          </h1>
          <h2 class="subtitle is-5 is-uppercase has-text-weight-light">
            Designer & Visual Artist
          </h2>
          <p style="margin-right: 3rem">
            Versatile artist asfsdf sdfsdf sd fsdf sdfsdfds fdsf sdfsdf dsf dsfdf dsfdsf 
          </p>
        </div>      
      </div>

  <!--card ui with grid-->
  <div class="columns">

    <div class="column">
      <figure class="column">
        <div class="home-card image">
          <div class="poster"><img src="https://bulma.io/images/placeholders/480x600.png" alt=""></div>

        </div>
          <h2 class="title is-4">My Humble Existence</h2>
          <h3 class="subtitle is-6">Drawings & Paintings</h3>
      </figure>
    </div>

    <div class="column">
      <figure class="column">
        <div class="home-card image">
          <div class="poster"><img src="https://bulma.io/images/placeholders/480x600.png" alt=""></div>

        </div>
          <h2 class="title is-4">Zooettes</h2>
          <h3 class="subtitle is-6">Graphic Design</h3>
      </figure>
    </div>

    <div class="column">
      <figure class="column">
        <div class="home-card image">
          <div class="poster"><img src="https://bulma.io/images/placeholders/480x600.png" alt=""></div>

        </div>
          <h2 class="title is-4">Welcome to Autumn</h2>
          <h3 class="subtitle is-6">3D, Illustration, World Building</h3>
      </figure>
    </div>

    <div class="column">
      <figure class="column">
        <div class="home-card image">
          <div class="poster"><img src="https://bulma.io/images/placeholders/480x600.png" alt=""></div>

        </div>
          <h2 class="title is-4">Cabells</h2>
          <h3 class="subtitle is-6">UI/UX, Branding, Data Vis</h3>
      </figure>
    </div>






  </div> 

  </div>   



   <!-- card ui
   <div class="home-card">
     <div class="poster"><img src="https://bulma.io/images/placeholders/480x600.png" alt=""></div>
     <div class="details">
      <h2>Title Goes Here<br><span>Subtitle Goes Here</span></h2>
      <div class="info">
        <p>Lorum ipsum sfsdf sdf sdf    sdfsdfsdfs sdf sdf sdf   s dfsdf sdf sdf sdfs </p>
      </div>
      </div>
   </div> -->

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

<style>
  .body {
    margin: 0;
    padding: 0;
    background: url("https://bulma.io/images/placeholders/480x600.png");
    background-size: cover;
  }

  .home-card {
    position: relative;
    border-radius: 12px;
    /* top: 50%; */
    /* left: 50%; */
    /* transform: translate(-50%, 0%); */
    /* width: 480px; */
    /* height: 600px; */
    margin-bottom: 2em;
    background: #000;
    overflow: hidden;
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.164);
  }

  /* .home-card .poster {
    position: relative;
    overflow: hidden;
  } */

  .home-card .poster img {
    width: 100%;
    transition: 0.2s;
  }

  .home-card:hover .poster img {
    filter: blur(5px);
    transform: translateY(-5px);
  }

  .home-card .poster:before {
    content: '';
    position: absolute;
    bottom: -180px;
    left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(0deg, #000 25%, transparent);
    transition: 0.5s;
    z-index: 1;
  }


</style>


