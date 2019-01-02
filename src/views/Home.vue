<template>
  <div class="home hero is-dark is-fullheight">


    
    <!--testing css grid-->
    <div class="grid">

      <aside class="sidebar-left">
            <figure class="image is-128x128">
              <img class="is-rounded" src="https://bulma.io/images/placeholders/128x128.png">
            </figure>
            <h1 class="title is-2">
              Ricky Colson III
            </h1>
            <h2 class="subtitle is-5 is-uppercase has-text-weight-light">
              Designer & Visual Artist
            </h2>
            <p>
              Versatile artist asfsdf sdfsdf sd fsdf sdfsdfds fdsf sdfsdf dsf dsfdf dsfdsf 
            </p>
      </aside>

      <article class="module">
        <div class="item">
          <figure class="column">
            <div class="home-card image">
              <div class="poster"><img src="https://bulma.io/images/placeholders/480x600.png" alt=""></div>
            </div>
            <h2 class="title is-4">My Humble Existence</h2>
            <h3 class="subtitle is-6">Drawings & Paintings</h3>
          </figure>
        </div>
        <div class="item">
          <figure class="column">
            <div class="home-card image">
              <div class="poster"><img src="https://bulma.io/images/placeholders/480x600.png" alt=""></div>
            </div>
            <h2 class="title is-4">My Humble Existence</h2>
            <h3 class="subtitle is-6">Drawings & Paintings</h3>
          </figure>
        </div>
        <div class="item">
          <figure class="column">
            <div class="home-card image">
              <div class="poster"><img src="https://bulma.io/images/placeholders/480x600.png" alt=""></div>
            </div>
            <h2 class="title is-4">My Humble Existence</h2>
            <h3 class="subtitle is-6">Drawings & Paintings</h3>
          </figure>
        </div>
        <div class="item">
          <figure class="column">
            <div class="home-card image">
              <div class="poster"><img src="https://bulma.io/images/placeholders/480x600.png" alt=""></div>
            </div>
            <h2 class="title is-4">My Humble Existence</h2>
            <h3 class="subtitle is-6">Drawings & Paintings</h3>
          </figure>
        </div>
      </article>

    </div>


		<!-- Footer -->
			<footer id="hero-foot">
				<div class="content has-text-centered">
          <p>
            Copyright 2019 Ricky Colson
          </p>
				</div>
			</footer>



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



/* grid */
.grid {
  display: grid;
  flex-wrap: wrap;
  grid-template-columns: 1fr 3fr;
  grid-gap: 2em;
  padding: 1em 4em;
  background: rgb(41, 41, 41);
  border: 1px solid red;
}

.grid * {
  border: 1px solid rgb(139, 0, 0);
}

@media all and (max-width: 1520px) {
  .grid {
    padding: 1em 1.5em;
  }
  aside,
  article {
    grid-column: 1 / 4;
  }
  .module {
    display: block;
  }
}

@media all and (max-width: 920px) {
  .grid {
    padding: 1em 0em;
  }
  aside {
    padding: 0em 1.5em;
  }
  .module {
    display: block;
    background: green;
    flex-wrap: wrap;
  }
  .item {
    flex: 1 1 50%; /* default 0 */
  }
}

@media all and (max-width: 600px) {
  .item {
    flex: 1 1 100%; /* default 0 */
  }
}

.module {
  /* Demo-Specific Styles */
  display: flex;
  align-items: center;
  justify-content: center;
  
  /* Flex Fallback */
  margin-left: 5px;
  margin-right: 5px;
  flex: 1 1 200px;
}

/* If Grid is supported, remove the margin we set for the fallback */
@supports (display: grid) {
  .module {
    margin: 0;
  }
}
</style>


