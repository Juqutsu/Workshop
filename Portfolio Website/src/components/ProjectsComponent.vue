<script setup>
</script>

<template>
    <main>
        <h1>Projects</h1>
        <hr>
        <div class="project-container">
            <a href="">
                <div class="item">
                    <h3>Serenity</h3>
                </div>
            </a>
            <a href="">
                <div class="item">
                    <h3>Portfolio</h3>
                </div>
            </a>
        </div>
    </main>
</template>

<style scoped>

main {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-color: #302F2F;
}

a {
    text-decoration: none;
}

hr {
    width: 5rem;
    margin-top: 5px;
    margin-bottom: 1rem;
}

.project-container {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 2rem;
}

.project-container .item {
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 8rem;
    width: 20rem;
    background-color: #252525;
    border-radius: 0.5rem;

}

.project-container .item h3 {
    margin-top: 0.5rem;
}




</style>