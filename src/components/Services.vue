<template>
    <section id="services" data-theme="dark">
        <div class="container">
            <hgroup>
                <h2>Serviços</h2>
                <h3></h3>
            </hgroup>
                <div class="grid">
                    <ServiceItem v-for="skill in skills" v-bind:key="skill"
                        :icon="skill.icon"
                        :item="skill.title"
                        :description="skill.description"
                    />
                </div>
        </div>
    </section>
</template>
<script>
import ServiceItem from '@/components/ServiceItem.vue'

export default {
    name:"ServicesHome",
    props:{
        skills:Array
    },
    components:{
        ServiceItem
    }

}
</script>
<style scoped>
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
