<template>
    <div class="container">

        <h1>lukas</h1>

        <nav>
            <a href="">Home</a>
            <a href="">About</a>
        </nav>

        <div class="icons">
            <a href=""><i class="pi pi-github"></i></a>
            <a href=""><i class="pi pi-youtube"></i></a>
            <a href=""><i class="pi pi-twitch"></i></a>
        </div>
    </div>
</template>

<style scoped>

.container {
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    align-items: center;
    background-color: #302F2F;
    height: 5rem;
}

h1 {
    color: white;
    font-weight: 500;
}

a {
    text-decoration: none;
    color: white;
}

nav {
    display: flex;
    gap: 20px;
}

.icons {
    display: flex;
    gap: 1rem;
}

</style>