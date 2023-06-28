<template>
    <div class="section-heading">
        <div class="section-title">
            <p>About Me</p>
        </div>
        <div class="section-line"></div>
    </div>

    <div class="container">
        <div class="about">
            <p>Hello! My name is Praneeth Ravuri, and I love developing websites. I started my coding journey in the year
                2020, right at the time of the COVID lockdown. I tinkered with Python first, made some small projects, and
                gained a strong grip on that language. I spent the remainder of the year creating simple bots to scrape
                e-commerce websites.</p>
        </div>

        <div class="about">
            <p>Later, I began building blogs on WordPress and blogger.com. As a result, I was appointed as a web developer
                for the IEEE student body of my university. I started learning HTML and CSS to enhance the user interface of
                the old website, but I almost gave up because I found CSS to be confusing. Nevertheless, after completing
                two
                internships in software and web development, I am now developing full-stack applications with a wide variety
                of use cases.</p>
        </div>

        <div class="about">
            <p>I am fueled by a burning passion for web development and I am more than ready to take on exciting full-time
                opportunities in the field! I am currently open to full-time opportunities, and my inbox is always open for
                connecting and networking. <span><a href="mailto: prav2500@gmail.com" class="about-contact-link">Feel free
                        to say hi!</a></span></p>
        </div>

    </div>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "About",
}
</script>

<style scoped lang="scss">
@import "@/styles/_variables.scss";

.container {

    margin-top: 20px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;

    & .about {
        width: 100%;

    }

    & div p {
        margin: 20px 0px;
        font-size: 1.125rem;

        @media only screen and (max-width: 600px) {
            font-size: 0.95rem;
        }

        @media only screen and (max-width: 320px) {
            font-size: 0.85rem;
        }
    }

}

.about-contact-link {
    text-decoration: none;
    color: $bright-red;
    transition: $transition;

    &:hover {
        color: $dark-red;
    }
}
</style>
  