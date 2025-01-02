<template>
    <nav data-theme="light">
        <ul></ul>
        <ul>
            <span v-for=" item in social_links" v-bind:key="item">
            <a target="_blank" rel="noopener noreferrer" :href="item.link">
                <i class="fab fa-2x socialicons" :class="item.icon"></i>
            </a>
            <li>&nbsp;</li>
            </span>
        </ul>
        <ul></ul>
    </nav>    
</template>


<script>

export default {
    name:"SocialMidia",
    props:{
        social_links:Array
        
    }
}
</script>
<style scoped>
nav{
    margin-bottom: 1em;
}

</style>