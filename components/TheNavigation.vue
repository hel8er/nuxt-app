<template>

    <nav class="nav">
        <div class="title">
            <h1><NuxtLink to="/">App Title</NuxtLink></h1>
        </div>

        <ul>
            <li><NuxtLink to="/">Home</NuxtLink></li>
            <li><NuxtLink to="/about">About</NuxtLink></li>
            <li><NuxtLink to="/contact">Contact</NuxtLink></li>
            <li><NuxtLink to="/test">Test API</NuxtLink></li>
        </ul>

    </nav>

</template>

<style scoped>
.nav {
    color: white;
    align-items: center;
    height: 48px;
    display: flex;
    background-color: rgb(46, 67, 160);
    justify-content: space-between;
}

.title {
    margin-left: 1rem;
}

ul {
    display: flex;
}

ul li {
    display: flex;
    margin-right: .5rem;

}
ul li :hover {
    color: rgb(226, 144, 21);
}
</style>