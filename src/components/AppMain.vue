<script>
import AppCard from "./AppCard.vue";

export default {
    name: "AppMain",
    components: {
        AppCard
    },
    data() {
        return {
            links: [
                {
                    title: "Discord",
                    description: "HTML e CSS, non responsive",
                    date: "7 Settembre",
                    href: "https://www.discord.morandiandrea.com",
                    github: "https://github.com/andreamorandi/htmlcss-discord",
                    color: "violet",
                },
                {
                    title: "Dropbox",
                    description: "HTML e CSS, non responsive",
                    date: "15 Settembre",
                    href: "https://www.dropbox.morandiandrea.com",
                    github: "https://github.com/andreamorandi/htmlcss-dropbox",
                    color: "light-blue",
                },
                {
                    title: "Spotify",
                    description: "HTML e CSS, web app responsive",
                    date: "23 Settembre",
                    href: "https://www.spotify.morandiandrea.com",
                    github: "https://github.com/andreamorandi/html-css-spotifyweb",
                    color: "green",
                },
                {
                    title: "Campo Minato",
                    description: "HTML, CSS e JavaScript, responsive",
                    date: "18 Ottobre",
                    href: "https://www.campominato.morandiandrea.com",
                    github: "https://github.com/andreamorandi/js-campominato-dom",
                    color: "dark-blue",
                },
                {
                    title: "WhatsApp",
                    description: "Vue, web app non responsive",
                    date: "8 Novembre",
                    href: "https://www.whatsapp.morandiandrea.com",
                    github: "https://github.com/andreamorandi/vue-boolzapp",
                    color: "light-green",
                },
                {
                    title: "Netflix",
                    description: "Vue + Vite + Sass, responsive",
                    date: "17 Novembre",
                    href: "https://www.boolflix.morandiandrea.com",
                    github: "https://github.com/andreamorandi/vite-boolflix",
                    color: "red",
                },
                {
                    title: "Progetto mid-term",
                    description: "Vue + Vite + Sass, responsive",
                    date: "24 Novembre",
                    href: "https://www.prgmidterm.morandiandrea.com",
                    github: "https://github.com/andreamorandi/proj-html-vuejs",
                    color: "yellow",
                },
            ],
        };
    },
};
</script>

<template>
    <main>
        <div class="container-md">
            <ul>
                <li v-for="(link, index) in links.slice().reverse()" :key="index">
                    <AppCard :link="link" />
                </li>
            </ul>
        </div>
    </main>
</template>

<style lang="scss" scoped>
main {
    padding-bottom: 2rem;
}
</style>