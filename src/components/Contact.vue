<template>
    <div class="section-heading">
        <div class="section-title">
            <p>Contact Me</p>
        </div>
        <div class="section-line"></div>
    </div>
    <form action="https://formspree.io/f/xvoneggn" method="POST">
        <label>
            Your email:
            <input type="email" name="email">
        </label>
        <label>
            Your message:
            <textarea name="message"></textarea>
        </label>
        <!-- your other form fields go here -->
        <button type="submit">Shoot &rarr;</button>
    </form>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Contact",
}
</script>

<style scoped lang="scss">
@import "@/styles/contact.scss";
</style>
  