<template>
    <nav data-theme="light">
        <ul></ul>
        <ul>
        <a target="_blank" rel="noopener noreferrer" :href="github" aria-label="davidbernardes">
            <i class="fab fa-github  fa-2x socialicons"></i>
        </a>
        <li>|</li>
        <a target="_blank" rel="noopener noreferrer" :href="linkedin" aria-label="My linkedin">
            <i class="fab fa-linkedin  fa-2x socialicons"></i>
        </a>
        <li>|</li>
        <a target="_blank" rel="noopener noreferrer" :href="email" aria-label="My linkedin">
            <i class="fas fa-envelope-square fa-2x"></i>
        </a>
        </ul>
        <ul></ul>
    </nav>    
</template>


<script>

export default {
    name:"SocialMidia",
    props:{
        github:{type:String, default:""},
        linkedin:{type:String, default:""},
        email:{type:String, default:""}
    }
}
</script>
<style scoped>
nav{
    margin-bottom: 1em;
}

</style>