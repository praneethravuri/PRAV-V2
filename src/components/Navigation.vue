<template>
    <nav class="navbar navbar-expand-lg">
        <div class="container-fluid">
            <a class="navbar-brand" href="#"><p class="prav-heading">PRAV</p></a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
                aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon" style="color: red"></span>
            </button>
            <div class="collapse navbar-collapse justify-content-center" id="navbarNav">
                <ul class="navbar-nav">
                    <li class="nav-item">
                        <a class="nav-link" href="#"><span class="db-slash">// </span>Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#"><span class="db-slash">// </span>Projects</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#"><span class="db-slash">// </span>Experience</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#"><span class="db-slash">// </span>Contact Me</a>
                    </li>
                </ul>
            </div>
            <a class="resume-btn" href="#">Resume</a>
        </div>
    </nav>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Navigation"
}
</script>

<style scoped lang="scss">
@import "@/styles/navigation.scss";
</style>