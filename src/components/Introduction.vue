<template>
    <div class="container">
        <div class="intro-text">
            <p><span class="telugu-text" v-on:mouseover="mouseover" v-on:mouseleave="mouseleave">{{message}}</span>, I'm</p>
        </div>

        <div class="name">
            <p class="name-text">Praneeth Ravuri</p>
        </div>

        <div class="description">
            <p class="desc">Graduate Computer Science Student at George Mason University</p>
            <p class="desc">Passionate about web development and software engineering</p>
        </div>

        <div class="location">
            <svg class="location-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
                <path
                    d="M12 0C7.304 0 3 4.304 3 9c0 1.54.424 2.996 1.155 4.255L12 24l7.845-10.746C20.576 11.996 21 10.54 21 9c0-4.696-4.304-9-9-9zm0 13a3 3 0 100-6 3 3 0 000 6z" />
            </svg>
            <p class="location-text">Fairfax, VA</p>
        </div>

        <div class="skills-container">
            <div class="skills" v-for="skill in skills" :key="skill">
                <p>{{ skill }}</p>
            </div>
        </div>

    </div>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Introduction",
    el : ".telugu-text",
    data() {
        return {
            skills: ["Python", "Javascript", "jQuery", "Express.js", "Node.js", "Vue.js", "Flask", "MongoDB", "Sass", "C"],
            message : "నమస్కారం"
        }
    },
    methods : {
        mouseover : function(){
            this.message = "Hello"
        },
        mouseleave: function(){
            this.message = "నమస్కారం"
        }
    }
}
</script>

<style lang="scss" scoped>
@import "@/styles/introduction.scss";
</style>