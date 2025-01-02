<template>
<div class="main">
    <HeaderHome
      :profile_name="profile.name"
      :picture="profile.picture"
      :specialty="profile.specialty"
    />
    <AboutHome
    :about="profile.about"
    :show_title=false
    />
    <SocialMidia
        :social_links="profile.social"
    />
    <ServicesHome
    :skills="profile.skills"
    />
    <ProjectsHome
      :projects="profile.projects"
    />
    <ToolsHome
      :tools="profile.tools"
    />
    <FooTer/>
</div>
</template>

<script>
import HeaderHome from '@/components/HeaderHome.vue'
import SocialMidia from '@/components/SocialMidia.vue'
import ToolsHome from '@/components/Tools.vue'
import AboutHome from '@/components/About.vue'
import ServicesHome from '@/components/Services.vue'
import ProjectsHome from '@/components/Projects.vue'
import FooTer from '@/components/FooTer.vue'

export default {
  name: 'HomeMain',
  props:{
    profile:Object
  },
  components:{
    HeaderHome,
    ToolsHome,
    AboutHome,
    ServicesHome,
    ProjectsHome,
    FooTer,
    SocialMidia
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


</style>
