<template>

    <div class="footer-content">
        <p>Designed and Built by Praneeth Ravuri</p>
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
        color: $bright-red;
        font-family: $source-code-pro-font;
        letter-spacing: -1px;
        border-top: 1px solid $dark-red;
        padding: 20px;
    }
}
</style>
  