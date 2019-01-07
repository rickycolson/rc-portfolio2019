<template>
  <div class="home hero is-dark is-fullheight">
    <div class="grid">
      <aside class="sidebar-left">
            <h1 class="title is-2">
              Ricky Colson III
            </h1>
            <h2 class="subtitle is-5 is-uppercase has-text-weight-light">
              Designer & Visual Artist
            </h2>
            <p>
              Versatile artist, product designer, generalist, Fort Collins Colorado, critical eye, tone/story, creative direction, asfsdf sdfsdf sd fsdf sdfsdfds fdsf sdfsdf dsf dsfdf dsfdsf 
            </p>
      </aside>
      <HomeProject/>
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
import HomeProject from '@/components/HomeProject.vue'

export default {
  name: 'home',
  components: {
    HelloWorld,
    HomeProject
  },
  
}
</script>

<style>
  .body {
    margin: 0;
    padding: 0;
    background: url("https://bulma.io/images/placeholders/480x600.png");
    background-size: cover;
  }

  /* grid */
  .grid {
    display: grid;
    flex-wrap: wrap;
    grid-template-columns: 1fr 3fr;
    grid-gap: 2em;
    padding: 1em 4em;
    background: rgb(41, 41, 41);
    border: 1px solid orange;
  }

  .grid * {
    border: 1px solid orange(139, 0, 0);
  }

  @media all and (max-width: 1520px) {
    .grid {
      padding: 1em 1.5em;
    }
    aside,
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


