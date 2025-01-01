<template>
    <section id="about" data-theme="light" >
        <div class="container">
            <hgroup v-if="show_title">

                <h2>Sobre</h2>
                <h3></h3>
            </hgroup>
            <p style="white-space: break-spaces;">{{ about }}</p>
        </div>
    </section>
</template>

<script>
export default {
    name:'AboutHome',
    props:{
        about:String,
        show_title:{
            default:true,
            type:Boolean,
        }

    }

}
</script>
<style scoped>
section{
    padding-top: 1.5em;
    background-color: var(--background-color);
    margin-bottom: 0px;
    text-align: justify;
}
hgroup::after{

    display: block;
    max-width: 100px;
    margin-top: 1rem;
    border-bottom: .125rem solid var(--primary);
    content: "";
}
</style>