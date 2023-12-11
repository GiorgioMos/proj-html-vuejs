<script>
export default {
    data() {
        return {
            sponsors: [
                { path: '../assets/img/client-logo-01.png' },
                { path: '../assets/img/client-logo-02.png' },
                { path: '../assets/img/client-logo-03.png' },
                { path: '../assets/img/client-logo-04.png' },
                { path: '../assets/img/client-logo-05.png' },
                { path: '../assets/img/client-logo-06.png' },
                { path: '../assets/img/client-logo-07.png' },
                { path: '../assets/img/client-logo-08.png' },
            ]
        }
    }
}
</script>

<template>
    <div class="jumbo">
        <div class="jumbo-items">
            <div class="text">
                <h2><b>Distant learning for further expansion</b></h2>
                <p>
                    Learning is a life-long journey that in fact we never find the terminate stop. Stop searching, enjoy the
                    process.
                </p>
            </div>
            <div class="download">
                <span><i class="fa-solid fa-download"></i></span>
                <span>Download Free Guide</span>
            </div>
            <div class="faq">
                <p>
                    Have questions? <span> <a href="#"> Get Free Sample <i
                                class="fa-solid fa-arrow-right fa-sm"></i></a></span>
                </p>
            </div>

        </div>

        <!-- aggiungi background e crea moving bg with mouse position -->

        <img src="../assets/img/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg" alt="jumbo-img">
    </div>

    <div v-for="sponsor in  sponsors " class="sponsors">
        <img :src="sponsor.path" alt="img">
    </div>
</template>

<style scoped lang="scss">
.jumbo {
    width: 100%;
    height: 800px;
    margin-top: 60px;
    padding: 0 7%;

    display: flex;
    justify-content: center;
    align-items: center;

    .jumbo-items {
        margin: 1rem;
        width: 400px;

        h2 {
            font-size: 40px;
        }

        .faq>p>span {
            color: #20AD96;
            text-decoration: underline;

            a {
                text-decoration: none;
                color: #20AD96;
            }
        }

    }

    img {
        width: 500px;
        border-radius: 50%;
        margin: 60px;
    }
}



span {
    margin: 4px;
}

.download:hover {
    background-color: #3F3A64;
    transition-duration: 0.3s;
}

.download {
    background-color: #20AD96;
    text-align: center;
    padding: 16px 0;
    border-radius: 10px;
    width: 250px;
}

h2,
p,
.download {
    margin-bottom: 30px;
}

.sponsors>img:hover {
    filter: brightness(50%);
    transition-duration: 0.3s;
}
</style>