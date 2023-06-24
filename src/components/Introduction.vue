<template>
    <div class="container">
        <div class="hi">
            <p class="hi-text"><span title="Hello" style="color: #FF4057;">నమస్కారం, </span>I'm</p>
        </div>

        <div class="name">
            <p class="name-text">Praneeth Ravuri</p>
        </div>

        <div class="description">
            <p class="desc-1">Master's in Computer Science Student at George Mason University</p>
            <p class="desc-2">Passionate about continuous learning and staying updated with the latest advancements in
                technology</p>
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
    data() {
        return {
            skills: ["Python", "Javascript", "jQuery", "Express.js", "Node.js", "Vue.js", "Flask", "MongoDB", "Sass", "C"]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "@/styles/introduction.scss";
</style>