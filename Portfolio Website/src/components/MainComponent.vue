<script lang="ts">

</script>

<template>
    <main>
        <div class="left">
            <img src="../assets/logo.jpg" alt="logo">
        </div>

        <div class="right">
            <h1>I'm Lukas</h1>
            <p class="title">Developer</p>

            <p>Hello I am Lukas, 19 years and <br>pro Valorant gamer und in <br>meiner Freizeit bin ich Spiderman</p>
        </div>
    </main>
</template>

<style scoped>

main {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    background-color: #302F2F;
    height: 30rem;
    gap: 4rem;
}

div.right {
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 1rem;
}

div.right .title {
    color: aqua;
}

div.left img {
    height: 14rem;
    width: 14rem;
    object-fit: cover;
    object-position: 50% 10%;
    border-radius: 50%;
}
</style>