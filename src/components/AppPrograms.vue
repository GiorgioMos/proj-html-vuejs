<script>
export default {
    data() {
        return {
            cards: [
                {
                    path: 'src/assets/img/home-2-image-box-01.png',
                    title: 'Customize Preferences',
                    description: 'Learners are given the right to arrange and customize their study schedule.',
                    link: 'Start here'
                },
                {
                    path: 'src/assets/img/about-us-02-image-box-02.png',
                    title: 'Cloud Storage',
                    description: 'You can store online lessons via online cloud or downloadto your device.',
                    link: 'Get Free Quote'
                },
                {
                    path: 'src/assets/img/home-2-image-box-03.png',
                    title: 'Multimedia Channels',
                    description: 'We provide study materials with various formats: video, audio and slides.',
                    link: 'Start Now'
                },
            ]
        }
    }
}
</script>

<template>
    <h3>MAXCOACH AVAILABLE COURSES</h3>
    <h2>Access <span>Smart Tutoring</span> Program For Benefits.</h2>
    <section class="card-flex">
        <div v-for="card in cards" class="card-container">
            <img :src="card.path" alt="img">
            <div class="card-info">
                <h4>{{ card.title }}</h4>
                <p>{{ card.description }}</p>
                <br>
                <a href="#">{{ card.link }} <i class="fa-solid fa-arrow-right"></i></a>
            </div>
        </div>
    </section>
    <section class="video-container">
        <div class="video">
            <iframe width="845" height="475" src="https://www.youtube.com/embed/ElFJ1qcl74U"
                title="Easily Customize Your Coaching Site With Elementor &amp; MaxCoach" frameborder="0"
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                allowfullscreen></iframe>
        </div>
        <div class="video-text">
            <h3>GET STARTED EFFORTLESSLY</h3>
            <h2>Enjoy out <br>Companionship</h2>
            <p>Sneek peek into what has in store for you on our online teaching and mentoring portal. Seek for some hidden
                hints of early-bird rewards as well.</p>
            <a href="#">Download free guidebook <i class="fa-solid fa-arrow-right"></i></a>
        </div>
    </section>
</template>

<style scoped lang="scss">
h2,
h3 {
    text-align: center;

}

span {
    color: #20AD96;
}

.card-flex {
    margin: 130px 20%;

    display: flex;
    justify-content: center;
}

.card-container {
    width: 350px;

    h4,
    p {
        margin: 20px 0;
    }
}

a {
    text-decoration: none;
}

.video-container {
    margin: 0 20%;

    display: flex;
    align-items: center;

    .video-text {
        width: 700px;
        margin-left: 70px;

        h2,
        h3,
        {
        margin: 26px 0;
    }

    p {
        margin-top: 30px;
        margin-bottom: 100px;
    }
}
}

iframe {
    width: 600px;
    height: 400px;
    border-radius: 6px;
}
</style>