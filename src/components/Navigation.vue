<template>
    <nav class="navbar navbar-expand-lg">
        <div class="container-fluid">
            <a class="navbar-brand prav-heading" href="#">PRAV</a>
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
                        <a class="nav-link" href="#projects"><span class="db-slash">// </span>Projects</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#experience"><span class="db-slash">// </span>Experience</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#contact"><span class="db-slash">// </span>Contact Me</a>
                    </li>
                    <li class="nav-item">
                        <a class="resume-btn" href="#"><span class="db-slash resume-slash">// </span>Resume</a>
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
@import "@/styles/navigation.scss";
</style>