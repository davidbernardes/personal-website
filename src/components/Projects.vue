<template>
    <section id="projects" data-theme="light">
        <div class="container">
            <hgroup>
                <h2>Projetos</h2>
                <h3></h3>
            </hgroup>
            <div class="grid">

                <div v-for="project in projects" v-bind:key="project">
                    <h6>{{project.title}}</h6>
                    <p>{{project.description}}</p>
                    <div style="text-align: end;">
                        <span v-for="tec in project.technologies" v-bind:key="tec">
                            <mark class="small_text" >
                                {{tec}}
                            </mark>&nbsp;
                        </span>
                    
                    </div>
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
.small_text{
    font-size: small;
    text-align: end;
}
</style>