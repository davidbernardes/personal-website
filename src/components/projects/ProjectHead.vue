<template>
        <hgroup :data-target="tag">
            <h2>{{title}}</h2>
            <h3>{{subtitle}}</h3>
        </hgroup>
</template>
<script>
export default {
    name:'ProjectHead',
    props:{
        title:String,
        subtitle:String,
        tag:String
    }
}
</script>
<style scoped>

</style>