<template>
    <div class="main-container">
        <div class="badge-heading">
            <h3>Badges</h3>
        </div>
        
        <div class="soft-skills">
            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://jayden220.github.io/hostedImages/images/comptia-a-ce-certification.1.png" alt="">
                </div>
            </div>

            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://jayden220.github.io/hostedImages/images/comptia-it-operations-specialist-cios-stackable-certification.png" alt="">
                </div>
            </div>

            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://jayden220.github.io/hostedImages/images/comptia-network-ce-certification.1.png" alt="">
                </div>
            </div>

            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://jayden220.github.io/hostedImages/cybersecurity-essentials.png" alt="">
                </div>
            </div>
            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://jayden220.github.io/hostedImages//images/operating-systems-basics.png" alt="">
                </div>
            </div>
            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://jayden220.github.io/hostedImages//images/linux-unhatched.png" alt="">
                </div>
            </div>
            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://jayden220.github.io/hostedImages/images/UIUX.png" alt="">
                </div>
            </div>
            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://jayden220.github.io/hostedImages/images/SCRUM.png" alt="">
                </div>
            </div>
            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://jayden220.github.io/hostedImages/images/python-essentials-1.1.png" alt="">
                </div>
            </div>
        </div>
        <!-- start of skills container -->
         <div class="skill-heading">

             <h2>Technical skills</h2>
         </div>
        <div class="tech-skills">
            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" alt="">
                </div>
            </div>

            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="">
                </div>
            </div>

            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-original-wordmark.svg" alt="">
                </div>
            </div>

            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="">
                </div>
            </div>

            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vuejs/vuejs-original-wordmark.svg" alt="">
                </div>
            </div>

            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original-wordmark.svg" alt="">
                </div>
            </div>

            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nodejs/nodejs-original-wordmark.svg" alt="">
                </div>
            </div>

            <div class="card">
                <span></span>
                <div class="content">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/azuresqldatabase/azuresqldatabase-original.svg" alt="">
                </div>
            </div>
        </div>
        <!-- end of Tech skills container -->

    </div>
</template>

{"qual":"Comptia A+ Certification","qualimg": "https://jayden220.github.io/hostedImages/images/comptia-a-ce-certification.1.png"},
{"qual":"Comptia IT Operations Specialist Stackable Certification","qualimg": "https://jayden220.github.io/hostedImages/images/comptia-it-operations-specialist-cios-stackable-certification.png"},
{"qual":"Comptia N+ Certification","qualimg": "https://jayden220.github.io/hostedImages/images/comptia-network-ce-certification.1.png"},
{"qual":"Cisco Cybersecurity","qualimg": "https://jayden220.github.io/hostedImages/cybersecurity-essentials.png"}



<script>
export default {

}
</script>

<style scoped>
.main-container {
    height: fit-content;
    background-color: rgb(0, 0, 0);
}

.tech-skills {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(20em, 1fr));
    place-items: center;
    gap: 1.5cqi;
}
.soft-skills {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(20em, 1fr)); /* Responsive layout */
    place-items: center;
    gap: 4.5cqi;
}
.badge-heading{
    color: #fff;
    padding: 3em;
}
.skill-heading{
    color: #fff;
    padding: 3em;
}

img {
    height: 3em;
}

.card {
    position: relative;
    width: 100px;
    /* color: #fff; */
    transition: 0.5s;
    border-radius: 0px;
    border: none;
    cursor: pointer;
    margin: .5em 0;
}

.card:hover {
    transform: translateY(-20px);
}

.card::before {
    content: '';
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    background: linear-gradient(90deg, #ffbc00, #ff0058);
    border-radius: 0em;
}

.card::after {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(45deg, #ffbc00, #ff0058);
    /* filter: blur(30px); */
}

.card span {
    position: absolute;
    top: 6px;
    left: 6px;
    right: 6px;
    bottom: 6px;
    z-index: 2;
    border-radius: 0em;
}

.card .content {
    position: relative;
    padding: 10px;
    z-index: 10;
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 800;
    font-size: 1.5em;
}

/* Media query for smaller screens */
@media (max-width: 650px) {
    .tech-skills {
        grid-template-columns: repeat(3, 1fr); /* Adjusts to fit 3 cards in a row */
        gap: 0.8cqi; /* Reduced gap between cards */
    }
    .soft-skills {
        grid-template-columns: repeat(2, 1.5fr); /* Adjusts to fit 3 cards in a row */
        gap: 0.8cqi; /* Reduced gap between cards */
    }

    .card {
        width: 40px; /* Smaller card width to fit three in a row */
    }

    img {
        height: 1em;
        width: 1em; /* Smaller images inside the cards */
    }
}
</style>

