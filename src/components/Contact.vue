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
@import "@/styles/_variables.scss";

form {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 20px;
}

label {
    display: flex;
    flex-direction: column;
    margin-bottom: 20px;
    width: 80%;
    color: $bright-red;
    font-weight: 600;
}

input[type="email"],
textarea {
    padding: 10px;
    font-size: 16px;
    background-color: $light-navy;
    border: none;
    color: $silver-sand;
    font-weight: 600;
    transition: $transition;
    box-shadow: 0 0 10px 0 rgba(0, 0, 0, 0.5);
    caret-color: $bright-red;

    &:focus {
        outline: none;
        background-color: $navy;
        box-shadow: none;
    }
}

button[type="submit"] {
    padding: 10px 20px;
    font-size: 16px;
    background-color: $navy;
    color: $bright-red;
    font-weight: bold;
    border: 1px solid $bright-red;
    transition: $transition;

    &:hover {
        box-shadow: 5px 5px $bright-red;
    }
}
</style>
  