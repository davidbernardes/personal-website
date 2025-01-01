<template>
    <header data-theme="light">
        <div class="container">
            <img :src="img" />
        </div>
        <div class="container">
            <h1>{{ profile_name.toUpperCase() }}</h1>
            <code>
                <small>{{ specialty }}</small>
            </code>
        </div>
    </header>
</template>
<script>

export default {
    name: 'HeaderHome',
    props:{
        profile_name:{
            type:String,
            default:'profile'
        },
        picture:String,
        specialty:String
    },
    data(){
        return {
            img:require('../info/'+this.picture)
        }
    }
}
</script>


<style scoped>
h1{
    margin-bottom: 0;
}
header{
    text-align: center;
    /*padding-top: var(--block-spacing-vertical) 90;*/
    background-color: var(--background-color);
    padding-top: 3em;
    padding-bottom: 1em;
    /*height: 100vh;*/
}
img {
    width: 13em;
    max-width: 100%;
    margin-left: auto;
    margin-right: auto;
    display: block;
}


</style>