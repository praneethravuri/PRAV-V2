<template>
    <div class="container">
        <div class="intro-text">
            <p><span class="telugu-text" v-on:mouseover="mouseover" v-on:mouseleave="mouseleave">{{ message }}</span>, I'm
            </p>
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
    el: ".telugu-text",
    data() {
        return {
            skills: ["Python", "Javascript", "jQuery", "Express.js", "Node.js", "Vue.js", "Flask", "MongoDB", "Sass", "C"],
            message: "నమస్కారం"
        }
    },
    methods: {
        mouseover: function () {
            this.message = "Hello"
        },
        mouseleave: function () {
            this.message = "నమస్కారం"
        }
    }
}
</script>

<style lang="scss" scoped>
.container {
    margin-top: 200px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    height: 100vh;
    width: 75%;

    & div {
        margin: 30px 0px 10px 0px;
        font-size: clamp(1rem, 1.5vw, 2rem);
        text-align: center;
    }

    & .name-text {
        font-size: clamp(6rem, 7vw, 8rem);
        line-height: 100%;
        font-weight: 600;
        text-shadow: 10px 0px black;
        font-family: $inter-font;
    }

    .desc {
        text-align: center;
    }

    .telugu-text {
        color: $bright-red;
        cursor: pointer;
    }

    .location {
        display: flex;
        align-items: center;
        justify-content: center;
        text-align: center;

        &-icon {
            width: 20px;
            height: 20px;
            margin-right: 5px;
            fill: $bright-red;
        }

        &-text {
            font-size: 18px;
            color: $bright-red;
        }
    }

    .skills {
        margin: 10px 0px;

        &-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        & p {
            font-weight: 600;
            color: $bright-red;
            font-size: 18px;
            margin-right: 20px;
        }
    }

    @media (max-width: 600px) {
        margin-top: 0px;

        & .name-text {
            font-size: clamp(5rem, 6vw, 7rem);
        }
    }
}
</style>