<template>
    <section>
        <div class="columns">
            <div v-for="project in projects" class="column">
                <div class="box">
                    <div class="content">
                        <h2 class="title is-3 ">{{ project.title }}</h2>
                        <p class="subtitle is-5">{{ project.description }}</p>
                        <div class="tags are-dark is-centered">
                            <span v-for="tag in project.tags"  class="tag is-info is-medium">{{ tag }}</span>
                        </div>
                        <ul class="bullet-list">
                            <li v-for="goal in project.goals">{{ goal }}</li>
                        </ul>
                    </div>
                    <div class="card-image center">
                        <img :src="project.img">
                    </div>
                    <router-link :to="project.routeURL"><a class="button is-medium is-fullwidth">View project</a>
                    </router-link>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'CabellsProject',
    data() {
        return {
            projects: [
                { 
                    id: 1, 
                    title: "Project 1", 
                    description: "description", 
                    img: "https://images.unsplash.com/photo-1546019170-335d69036b46?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80", 
                    goals: [
                        "goal1", 
                        "goal2"
                    ],
                    tags: [
                        "UI/UX",
                        "Marketing"
                    ],
                    routeURL: "/project1"
                },
                { 
                    id: 2, 
                    title: "Project 2", 
                    description: "description", 
                    img: "https://images.unsplash.com/photo-1546029115-712217181a58?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80",
                    goals: [
                        "goal2.1", 
                        "goal2.2"
                    ],
                    tags: [
                        "UI/UX",
                        "Marketing"
                    ],
                    routeURL: "/project2"
                },
                { 
                    id: 3, 
                    title: "Project 3", 
                    description: "description", 
                    img: "https://images.unsplash.com/photo-1546029115-712217181a58?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80",
                    goals: [
                        "goal3.1", 
                        "goal3.2",
                        "goal3.3"
                    ],
                    tags: [
                        "UI/UX",
                        "Marketing"
                    ],
                    routeURL: "/project3"
                },
            ]
        }
    }
}
</script>

<style>
    ul {
        list-style-type: none;
    }

    .bullet-list {
        list-style-type: disc;
    }
</style>