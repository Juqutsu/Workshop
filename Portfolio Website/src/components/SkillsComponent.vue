<template>
    <main>
        <h1>Skills</h1>
        <hr>
        <div class="skills">
            <div class="skill" v-for="skill in skills" :key="skill.name">
                <a>{{ skill.name }}</a>
                <img :src="getImagePath(skill.path)" alt="skill image" class="skill-img">
                <div class="star-container">
                    <img v-for="n in skill.stars" :key="n" src="../assets/star.png" alt="star" class="star">
                </div>
            </div>
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
    color: white;
    padding: 2rem;
}
hr {
    width: 5rem;
    margin-top: 5px;
    margin-bottom: 1rem;
}
.skills {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 1rem;
}
.skill {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 7rem;
    width: 7rem;
    border: 1px solid white;
    border-radius: 1rem;
    padding: 1rem;
    background-color: #3A3A3A;
    text-align: center;
}
.skill a {
    color: white;
    text-decoration: none;
    margin-bottom: 0.5rem;
}
.skill-img {
    height: 3rem;
    width: 3rem;
    margin-bottom: 0.5rem;
}
.star-container {
    display: flex;
    justify-content: center;
    align-items: center;
}
.star {
    width: 1rem;
    height: 1rem;
    margin: 0 0.1rem;
}
</style>

<script>
export default {
    data() {
        return {
            skills: [
                { name: 'HTML', path: 'src/assets/html.png', stars: 4 },
                { name: 'CSS', path: 'src/assets/css.png', stars: 4 },
                { name: 'JavaScript', path: "src/assets/js.png", stars: 2 },
                { name: 'Tailwind CSS', path: 'src/assets/tailwind.png', stars: 4 },
                { name: 'Vue.js', path: 'src/assets/vue.png', stars: 3 },
                { name: 'Node.js', path: 'src/assets/node.png', stars: 3 }
            ]
        };
    },
    methods: {
        getImagePath(path) {
            return path ? path : '../assets/default.png';
        }
    }
};
</script>
