<template>
      <article class="module">
        <div v-for="project in projects" class="item">
          <figure class="column">
            <div class="home-card image">
              <div class="poster"><img :src="project.img" alt=""></div>
            </div>
            <h2 class="title is-4">{{ project.title }}</h2>
            <h3 class="subtitle is-6">{{ project.subtitle }}</h3>
            <span v-for="tag in project.tags" class="tag">{{ tag }}</span>
            <p>{{ project.description }}</p>
            <a v-if="project.href" :href="project.href" class="button is-text has-text-link">{{ project.CTA }}</a>
            <router-link :to="project.routeURL" class="button is-text has-text-link">{{ project.CTA }}</router-link>        
          </figure>
        </div>
      </article>
</template>

<script>
export default {
  name: 'HomeProject',
  data() {
          return {
              projects: [
                  { 
                      id: 1, 
                      title: "My Humble Existence", 
                      subtitle: "Drawings & Paintings", 
                      description: "This is a summary of the project and relevant skills", 
                      img: "https://bulma.io/images/placeholders/480x600.png",
                      tags: [
                          "personal"
                      ],
                      routeURL: "/my-humble-existence",
                      CTA: "View portfolio -->"
                  },
                  { 
                      id: 2, 
                      title: "Zooettes", 
                      subtitle: "Graphic Design", 
                      description: "This is a summary of the project and relevant skills", 
                      img: "https://bulma.io/images/placeholders/480x600.png",
                      tags: [
                          "personal"
                      ],
                      href: "http://zooettes.com",
                      CTA: "Visit site -->"
                  },
                  { 
                      id: 3, 
                      title: "Welcome to Autumn", 
                      subtitle: "World Building, 3d, Illustration", 
                      description: "This is a summary of the project and relevant skills", 
                      img: "https://bulma.io/images/placeholders/480x600.png",
                      tags: [
                          "personal"
                      ],
                      href: "http://welcometoautumn.com",
                      CTA: "Visit site -->"
                  },
                  { 
                      id: 4, 
                      title: "Cabells", 
                      subtitle: "Branding, UI/UX & Product Design", 
                      description: "This is a summary of the project and relevant skills", 
                      img: "https://bulma.io/images/placeholders/480x600.png",
                      tags: [
                          "team"
                      ],
                      routeURL: "/Cabells",
                      CTA: "View project -->"
                  },
                  
              ]
          }
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
  border: 11px solid orange;
}

.grid * {
  border: 1px solid rgb(247, 0, 226);
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


