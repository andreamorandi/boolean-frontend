<script>
export default {
    name: "AppCard",
    props: {
        link: Object,
    },
};
</script>

<template>
    <div class="card" :class="`bg-${link.color}`">
        <h3>{{  link.date }}</h3>
        <h2>{{ link.title }}</h2>
        <h4>{{ link.description }}</h4>
        <div class="links">
            <a :href="link.github">
                <i class="fa-brands fa-github"></i>
            </a>
            <a :href="link.href">
                <i class="fa-solid fa-globe"></i>
            </a>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.card{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: .5rem;
    margin: 2.5rem 1rem;
    padding: 1rem;
    border-radius: 10px;
    color: white;
    h3 {
        align-self: flex-start;
    }
    a {
        display: inline-block;
        margin: .75rem 2rem;
        i {
            font-size: 2.5rem;
            color: white;
        }
    }
}
</style>