<template>
    <section id="projects" data-theme="light">
        <div class="container">
            <hgroup>
                <h2>Projetos</h2>
                <h3></h3>
            </hgroup>
            <div class="grid">

                <div v-for="project in projects" v-bind:key="project">
                    <h6>Projeto</h6>
                    <p>Descriçaõ do projeto</p>
                    <hr>
                </div>
            </div>

            
        </div>
    </section>
</template>

<script>

export default {
    name:'ProjectsHome',
    props:{
        projects:Array
    }
}
</script>
<style scoped>
section{
    padding-top: 3em;
    background-color: var(--background-color);
    margin-bottom: 0px;
    padding-bottom: 3em;
}
hgroup::after{

    display: block;
    max-width: 100px;
    margin-top: 1rem;
    border-bottom: .125rem solid var(--primary);
    content: "";
}
</style>