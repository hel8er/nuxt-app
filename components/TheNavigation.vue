<template>

    <nav class="nav">
        <div class="title">
            <h1>App Title</h1>
        </div>

        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Contact</a></li>
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
</style>