<script>
export default {
    data() {
        return {
            cards: [
                {
                    path: 'src/assets/img/stock-full-hd-03-480x298.jpg',
                    title: 'Free',
                    pres: 'Personal Finance: Finantial Security Thinking & Principles',
                    lessons: '2 lessons',
                    students: '294 Students'
                },
                {
                    path: 'src/assets/img/stock-full-hd-03-480x298.jpg',
                    title: '$40.00',
                    pres: 'Personal Finance: Finantial Security Thinking & Principles',
                    lessons: '2 lessons',
                    students: '294 Students'
                },
                {
                    path: 'src/assets/img/stock-full-hd-03-480x298.jpg',
                    title: 'Free',
                    pres: 'Personal Finance: Finantial Security Thinking & Principles',
                    lessons: '2 lessons',
                    students: '294 Students'
                },
                {
                    path: 'src/assets/img/stock-full-hd-04-480x298.jpg',
                    title: '$19.00',
                    pres: 'Personal Finance: Finantial Security Thinking & Principles',
                    lessons: '2 lessons',
                    students: '294 Students'
                },
                {
                    path: 'src/assets/img/stock-full-hd-05-480x298.jpg',
                    title: '$26.00',
                    pres: 'Personal Finance: Finantial Security Thinking & Principles',
                    lessons: '2 lessons',
                    students: '294 Students'
                },
                {
                    path: 'src/assets/img/stock-full-hd-06-480x298.jpg',
                    title: '$39.00',
                    pres: 'Personal Finance: Finantial Security Thinking & Principles',
                    lessons: '2 lessons',
                    students: '294 Students'
                },
            ]
        }
    }
}
</script>

<template>
    <h3>STIMULATED TO LEARN?</h3>
    <h2>Featured Online Courses</h2>
    <section>
        <div v-for="card in cards" class="card-container">
            <img :src="card.path" alt="img">
            <div class="course-info">
                <h4>{{ card.title }}</h4>
                <p>{{ card.pres }}</p>
                <span class="card-footer"><i class="fa-solid fa-file-lines"></i>{{ card.lessons }}</span>
                <span class="card-footer"><i class="fa-regular fa-user"></i>{{ card.students }}</span>
            </div>
        </div>
    </section>
    <div class="download">
        <span><i class="fa-solid fa-download"></i></span>
        <span>Download Free Guide</span>
    </div>
</template>

<style scoped lang="scss">
h2,
h3 {
    text-align: center;
    margin: 30px 0;
}

section {
    display: flex;
    flex-wrap: wrap;
    margin: 0 7%;
}

.card-container {
    width: 600px;
    background-color: grey;
    margin: 40px 100px;
    height: 150px;
    border-radius: 5px;

    display: flex;

    img {
        clip-path: circle();
        width: 200px;
        height: 130px;
        margin-top: 10px;
    }

    .course-info {
        margin-top: 20px;

        h4,
        p,
        {
        margin-bottom: 12px;
    }

    p {
        margin-bottom: 20px;
        width: 300px;
    }

    .card-footer {
        margin: 0 30px;
    }
}
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
    margin: 50px 44%;
    margin-bottom: 150px;

    display: flex;
    justify-content: center;
    align-items: center;
}
</style>