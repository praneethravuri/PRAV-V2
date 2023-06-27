<template>
    <div class="section-heading">
        <div class="section-title">
            <p>Projects</p>
        </div>
        <div class="section-line"></div>
    </div>

    <p class="disclaimer"><span>Disclaimer:</span> Some project source code is unavailable due to its association with GMU
        courses and to uphold the integrity of the <span><a href="https://oai.gmu.edu/full-honor-code-document/"
                target="_blank">GMU Honor Code</a></span></p>

    <div class="card-grid">
        <div v-for="project in projects" :key="project.projectName" class="card" @click="redirectToLink(project)">
            <div class="card-images">
                <img src="../assets/images/code.svg" alt="Image 1" class="left-image">
                <div class="card-images-right">
                    <a v-if="project.githubLink" :href="project.githubLink" target="_blank" @click.stop>
                        <img src="../assets/images/github_bright_red.svg" alt="Image 2" class="right-image">
                    </a>
                    <a v-if="project.websiteLink" :href="project.websiteLink" target="_blank" @click.stop>
                        <img src="../assets/images/external-link.svg" alt="Image 3" class="right-image">
                    </a>
                </div>
            </div>
            <h3 class="card-name">{{ project.projectName }}</h3>
            <p class="card-description">{{ project.projectDescription }}</p>
            <div class="card-tags">
                <span v-for="tag in project.tags" :key="tag" class="tag">{{ tag }}</span>
            </div>
        </div>
    </div>
</template>
  
<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Projects",
    data() {
        return {
            projects: [
                {
                    projectName: "PRAV V2",
                    projectDescription:
                        "Second iteration of my personal website designed with Vue.js and Scss and hosted on Netlify",
                    githubLink: "https://github.com/praneethravuri/PRAV-V2",
                    websiteLink: "https://prav.dev/",
                    tags: ["Vue.js", "Javascript", "Scss"],
                },
                {
                    projectName: "PRAV",
                    projectDescription:
                        "First iteration of my personal website designed on the fly with Sass and Vanilla Javascript and hosted on Netlify",
                    websiteLink: "https://prav-v1.netlify.app/",
                    githubLink: "https://github.com/praneethravuri/PRAV",
                    tags: ["Javascript", "Sass", "jQuery"],
                },
                {
                    projectName: "Weatherly",
                    projectDescription: "Weatherly is a user-friendly website that seamlessly integrates with Google Maps to provide you with accurate and up-to-date weather information for any location around the world ",
                    websiteLink: "https://weatherly-google.netlify.app/",
                    tags: ["Javascript", "Sass", "jQuery"]
                },
                {
                    projectName: "Horizon Airlines Bookings",
                    projectDescription: "A full-stack application built using Flask and MongoDB to book and manage flight reservations. This application was created for the INFS 750 course at GMU",
                    githubLink: "https://github.com/praneethravuri/Horizon-Airlines-Bookings",
                    tags: ["Javascript", "Flask", "MongoDB", "Bootstrap"]
                },
                {
                    projectName: "Patriot Board",
                    projectDescription: "A collaborative project designed to improve the UI of GMU's course registration website",
                    githubLink: "https://github.com/praneethravuri/Patriot-Board",
                    websiteLink: "http://mason.gmu.edu/~kdonapat/index",
                    tags: ["Javascript", "Selenium", "jQuery"]
                },
                {
                    projectName: "Invespo",
                    projectDescription: "Invespo: A stock trading front-end for SWE 632 course @ George Mason Univ. Built with HTML, CSS, JS, jQuery. Explores interface design principles in user-centric design",
                    githubLink: "https://github.com/praneethravuri/Invespo",
                    tags: ["Javascript", "jQuery", "Bootstrap"]
                },
                {
                    projectName: "Jet Sphere",
                    projectDescription: "A backend web application with JWT user authentication and validation, manage flight bookings, update / delete account, administrative database changes, and session management",
                    githubLink: "https://github.com/praneethravuri/Jet-Sphere",
                    tags: ["Javascript", "MongoDB", "Node", "Express.js"]
                },
                {
                    projectName: "Amazon Product Information Scraper",
                    projectDescription: "A web-scraping bot that retrieves product names, prices, review stars, and review counts for a specific category",
                    githubLink: "https://github.com/praneethravuri/Amazon-Product-Information-Scraper",
                    tags: ["Python", "Selenium", "BeautifulSoup"]
                },
                {
                    projectName: "Task Tracker",
                    projectDescription: "A frontend project made with Vue.js. Includes functions like add, update, and delete tasks and toggle set reminders",
                    githubLink: "https://github.com/praneethravuri/Task-Tracker",
                    tags: ["Vue.js", "Javascript"]
                }

            ],
        };
    },
    methods: {
        redirectToLink(project) {
            if (project.websiteLink) {
                window.open(project.websiteLink, "_blank");
            } else if (project.githubLink) {
                window.open(project.githubLink, "_blank");
            }
        }
    }

};
</script>
  
<style scoped lang="scss">
@import "@/styles/_variables.scss";

.card-grid {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    gap: 20px;
    margin: 20px 0px;
}

.card {
    padding: 20px;
    background-color: $light-navy;
    height: 350px;
    box-shadow: 0 0 10px 0 rgba(0, 0, 0, 0.5);
    transition: $transition;
    cursor: pointer;

    &:hover {
        transform: translateY(-7px);
    }

    &-images {
        display: flex;
        justify-content: space-between;
        margin-bottom: 10px;
    }

    &-name {
        font-size: 1.5rem;
        margin: 0;
        color: $bright-red;
        font-weight: 600;
        margin-top: 20px;
    }

    &-description {
        margin: 10px 0;
        height: 90%;
        color: $silver-sand;
    }

    &-tags {
        display: flex;
        flex-wrap: wrap;
    }
}

.right-image,
.left-image {
    width: 30px;
    height: 30px;
    margin-right: 10px;
}

.tag {
    font-size: 1rem;
    color: #fff;
    margin-right: 20px;
    margin-bottom: 5px;
    color: $bright-red;
}

.disclaimer {
    margin-top: 20px;
    font-size: 15.5px;

    & span,
    & a {
        color: $bright-red;
        transition: $transition;

        text-decoration: none;
    }

    & a:hover {
        color: $dark-red;
    }
}

@media (min-width: 768px) {
    .card-grid {
        grid-template-columns: repeat(2, 1fr);
    }
}

@media (min-width: 1024px) {
    .card-grid {
        grid-template-columns: repeat(3, 1fr);
    }
}

@media (max-width: 600px) {
    .card-description {
        font-size: 14px
    }
}
</style>
  