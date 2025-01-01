<template>
    <footer class="container-fluid" data-theme="light">

            <small>
                <p>© DAVID BERNARDES JR |
                ALL RIGHTS RESERVED</p>
            </small>
    </footer>
</template>
<script>
//import SocialMidia from '@/components/SocialMidia.vue'

export default {
    name:'FooTer',
    props:{
        social:Object
    },
    components:{
        //SocialMidia
    }
}
</script>
<style>
footer{
    display: block;
    padding-top: 3em;
    height: 6em;
    background-color: var(background-color);
    text-align: center;
}
hr{
    margin-bottom: 2em;
}
</style>
