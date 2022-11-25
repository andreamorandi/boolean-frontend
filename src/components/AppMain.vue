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
                    href: "/discord",
                    github: "https://github.com/andreamorandi/htmlcss-discord",
                },
                {
                    title: "Dropbox",
                    description: "HTML e CSS, non responsive",
                    date: "15 Settembre",
                    href: "/dropbox",
                    github: "https://github.com/andreamorandi/htmlcss-dropbox",
                },
                {
                    title: "Spotify",
                    description: "HTML e CSS, web app responsive",
                    date: "23 Settembre",
                    href: "/spotify",
                    github: "https://github.com/andreamorandi/html-css-spotifyweb",
                },
                {
                    title: "Campo Minato",
                    description: "HTML, CSS e JavaScript, responsive",
                    date: "18 Ottobre",
                    href: "/campominato",
                    github: "https://github.com/andreamorandi/js-campominato-dom",
                },
                {
                    title: "WhatsApp",
                    description: "Vue, web app non responsive",
                    date: "8 Novembre",
                    href: "/whatsapp",
                    github: "https://github.com/andreamorandi/vue-boolzapp",
                },
                {
                    title: "Netflix",
                    description: "Vue + Vite + Sass, responsive",
                    date: "17 Novembre",
                    href: "/netflix",
                    github: "https://github.com/andreamorandi/vite-boolflix",
                },
                {
                    title: "Progetto mid-term",
                    description: "Vue + Vite + Sass, responsive",
                    date: "24 Novembre",
                    href: "/prgmidterm",
                    github: "https://github.com/andreamorandi/proj-html-vuejs",
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

</style>