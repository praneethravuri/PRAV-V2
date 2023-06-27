<template>
    <nav class="navbar navbar-expand-lg">
        <div class="container-fluid">
            <a class="navbar-brand prav-heading" href="">PRAV</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
                aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="hamburger-menu">&#9776;</span>
            </button>
            <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
                <ul class="navbar-nav ml-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="#navigation"><span class="db-slash">// </span>Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#about"><span class="db-slash">// </span>About Me</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#experience"><span class="db-slash">// </span>Experience</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#projects"><span class="db-slash">// </span>Projects</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#contact"><span class="db-slash">// </span>Contact Me</a>
                    </li>
                    <li class="nav-item">
                        <a class="resume-btn"
                            href="https://drive.google.com/file/d/1AiUdUmqhrWz8wlmGVeOhDD2Pr5CBxW7C/view?usp=sharing"
                            target="_blank"><span class="db-slash resume-slash">// </span>Resume</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Navigation",
    methods: {
        scrollToSection(sectionId) {
            // eslint-disable-next-line no-undef
            VueScrollTo.scrollTo(`#${sectionId}`, 500, {
                easing: 'ease-in',
                offset: -50, // Optional offset in pixels
            });
        },
    },
}
</script>

<style scoped lang="scss">
@import "@/styles/_variables.scss";

nav {
    padding: 20px;
    font-family: $source-code-pro-font;
    position: fixed;
    background-color: $dark-blue;
    width: 100%;
    z-index: 999;
    top: 0;

    .nav-link {
        color: $bright-red;
        font-size: 18px;
        margin: 0 10px;
        transition: $transition;

        &:hover {
            color: $dark-red;
        }
    }

    .db-slash {
        color: $slate;
        font-weight: bold;
    }

    .resume {
        &-slash {
            display: none;
        }

        &-btn {
            border: 1px solid $bright-red;
            padding: 10px 15px;
            color: $bright-red;
            text-decoration: none;
            transition: $transition;

            &:hover {
                box-shadow: 5px 5px $bright-red;
            }
        }

    }

    .prav-heading {
        font-size: 2rem;
        color: $bright-red;
        font-style: italic;
        font-weight: bold;
        transition: $transition;

        &:hover {
            color: $slate;
        }
    }

    .hamburger-menu {
        color: $bright-red;
    }

    @media (max-width: 1000px) {
        .resume-btn {
            margin: 0 10px;
            border: none;
            font-size: 18px;
            padding: 0;

            &:hover {
                box-shadow: none;
            }
        }

        .resume-slash {
            display: inline;
        }

        .hamburger-menu:focus {
            border: none;
        }

        .db-slash {
            display: none;
        }
    }
}
</style>