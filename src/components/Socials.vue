<template>
    <div class="socials-div">
        <div class="logo-div">
            <a href="mailto:prav2500@gmail.com" target="_blank"><img src="../assets/images/email_bright_red.svg"
                    alt="email logo" class="logo"></a>
        </div>
        <div class="logo-div">
            <a href="https://github.com/praneethravuri" target="_blank"><img src="../assets/images/github_bright_red.svg"
                    alt="github logo" class="logo"></a>
        </div>
        <div class="logo-div">
            <a href="https://www.linkedin.com/in/praneeth-ravuri2500/" target="_blank"><img
                    src="../assets/images/linkedin_bright_red.svg" alt="linkedin logo" class="logo"></a>
        </div>

        <div class="vertical-line"></div>
    </div>
</template>

<script>

export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Socials"
}
</script>

<style lang="scss" scoped>
@import "@/styles/_variables.scss";

.vertical-line {
    width: 1px;
    height: 25%;
    background-color: $bright-red;
}


.socials-div {
    position: fixed;
    bottom: 0;
    left: 0;
    width: 10%;
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    align-items: center;

    @media (max-width: 600px) {
        display: none;
    }
}


.logo {
    width: 35px;
    margin: 10px;
    transition: $transition;

    &-div {
        width: 100%;
        text-align: center;
        margin-bottom: 10px;
    }

    &:hover {
        transform: translateY(-7px);
        border: none;
    }
}</style>