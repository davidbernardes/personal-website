<template>
    <div class="container">
        <img :src="src_img" :alt="alt_img">
    </div>
</template>
<script>
export default{
    name:'ProjectImage',
    props:{
        src_img:String,
        alt_img: String
    }
}
</script>
<style scoped>
img{
    margin-top: 2em;
}

</style>