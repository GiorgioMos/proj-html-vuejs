<script>
export default {
    data() {
        return {
            NavItems: [
                { name: 'Home' },
                { name: 'Pages' },
                { name: 'Courses' },
                { name: 'Features' },
                { name: 'Blog' },
                { name: 'Shop' }
            ]
        }
    }
}
</script>

<template>
    <div id="nav">
        <a href="#"><img src="../assets/img/dark-logo.png" alt="Logo"></a>
        <ul>
            <li v-for="NavItem in NavItems">{{ NavItem.name }} <i class="fa-solid fa-angle-down fa-2xs"></i></li>
        </ul>
        <a class="user-icon" href="#"><i class="fa-regular fa-circle-user fa-lg"></i></a>
        <input type="text" placeholder="Search..." name="search">
        <button type="submit"><i class="fa-solid fa-magnifying-glass"></i></button>
    </div>
</template>

<style scoped lang="scss">
#nav {
    display: flex;
    height: 70px;
    box-shadow: 0px 10px 30px #F5F1ED;
    justify-content: center;
    align-items: center;
    padding: 0 7%;

    img {
        width: 150px;
        margin-right: 150px;
    }

    input {
        margin-left: 20px;
    }

    .user-icon {
        color: #20AD96;
    }

}

ul {
    list-style-type: none;
    display: flex;
    padding: 0;

    li {
        margin: 1rem;
    }
}
</style>
