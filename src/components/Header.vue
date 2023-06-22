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
    name: "Header"
}
</script>

<style scoped>

nav{
    padding: 20px;
    font-family: 'Source Code Pro', monospace;
}

.nav-link {
    color: #FF4057;
    font-size: 18px;
    transition: all 0.3s ease 0s;
    margin: 0px 10px;
}

.nav-link:hover {
    color: #9d2836;
}

.db-slash{
    color: #e6f1ff;
    font-weight: bold;
}

.resume-btn{
    border: 1px solid #FF4057;
    padding: 10px 15px;
    border-radius: 3px;
    color: #FF4057;
    text-decoration: none;
    transition: all 0.3s ease 0s;
}

.resume-btn:hover{
    box-shadow: 5px 5px #FF4057;
}

.prav-heading{
    font-size: 2rem;
    color: #FF4057;
    font-style: italic;
    font-weight: bold;
    transition: all 0.3s ease 0s;
}

.prav-heading:hover{
    color: #e6f1ff;
}

</style>