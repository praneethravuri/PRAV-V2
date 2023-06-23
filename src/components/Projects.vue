<template>
    <div class="section-heading">
        <div class="section-title">
            <p>Projects</p>
        </div>
        <div class="section-line"></div>
    </div>

    <div class="card-grid">
        <div class="card">
            <div class="card-images">
                <img src="../assets/images/code.svg" alt="Image 1" class="left-image">
                <div class="card-images-right">
                    <a href="https://github.com/praneethravuri/PRAV" target="_blank"><img src="../assets/images/github_bright_red.svg" alt="Image 2" class="right-image"></a>
                    <a href="https://prav.dev/" target="_blank"><img src="../assets/images/external-link.svg" alt="Image 3" class="right-image"></a>
                </div>
            </div>
            <h3 class="card-name">PRAV</h3>
            <p class="card-description">First iteration of my personal website made using Sass and Vanilla Javascript. Contains dynamically generated content and clear user interface</p>
            <div class="card-tags">
                <span class="tag">Javascript</span>
                <span class="tag">Sass</span>
                <span class="tag">jQuery</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Projects"
}
</script>

<style scoped lang="scss">
@import "@/styles/projects.scss";
</style>