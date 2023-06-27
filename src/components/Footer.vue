<template>

    <div class="footer-content">
        <p>Designed and Built by Praneeth Ravuri</p>

        <div class="social-links">
            <a href="https://www.linkedin.com/in/praneeth-ravuri2500/" target="_blank">LinkedIn</a>
            <span> | </span>
            <a href="https://github.com/praneethravuri" target="_blank">Github</a>
        </div>

        <p style="font-size: 12px; border: none;">2023 &copy; All Rights Reserved</p>

    </div>
</template>

<script>
export default{
    // eslint-disable-next-line vue/multi-word-component-names
    name : "Footer",
}
</script>

<style scoped lang="scss">
@import "@/styles/_variables.scss";

.footer-content {
    text-align: center;
    padding: 30px;
    z-index: 999;

    & p {
        color: $slate;
        letter-spacing: -1px;
        border-top: 1px solid $dark-red;
        padding: 20px;
    }

    span{
        font-weight: bold;
        color: $slate;
    }

    .social-links a{
        color: $bright-red;
        text-decoration: none;
        transition: $transition;

        &:hover{
            color: $dark-red;
        }
    }
}
</style>
  