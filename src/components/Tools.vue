<template>
    <section id="services" data-theme="dark">
        <div class="container">
            <hgroup>
                <h2>Ferramentas</h2>
                <h3></h3>
            </hgroup>
            <kbd v-for="tool in tools" v-bind:key="tool">
                <small>{{tool}}</small>
            </kbd>
    
        </div>
    </section>
</template>
<script>

export default {
    name: 'ToolsHome',
    props:{
        tools:Array
    },
    components:{

    }
}
</script>


<style scoped>

header{
    text-align: center;
    /*padding-top: var(--block-spacing-vertical) 90;*/
    background-color: var(--background-color);
    padding-top: 3em;
    padding-bottom: 1em;
    /*height: 100vh;*/
}

kbd{
    margin: .1em;
}
section{
    padding-top: 3em;
    padding-bottom: 2em;
    background-color: var(--background-color);
    margin-bottom: 0px;
}
hgroup::after{

    display: block;
    max-width: 100px;
    margin-top: 1rem;
    border-bottom: .125rem solid var(--primary);
    content: "";
}

</style>