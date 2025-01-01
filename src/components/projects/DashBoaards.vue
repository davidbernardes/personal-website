<template>
    <article>
        <ProjectHead 
        :data-target="tag" 
        :title="title"
        :subtitle="subtitle"
        @click="open_modal($event)"
        />
        <!-- Modal -->
        <img src="" alt="">
        <dialog :id="tag">
              <article>
                  <a href="#close"
                  aria-label="Close"
                  class="close"
                  :data-target="tag"
                  @click="close_modal($event)">
                </a>
                
                <div class="container">
                  <hgroup>
                    <h2>{{title}}</h2>
                    <h3>{{subtitle}}</h3>
                  </hgroup>
        
                  <p>
                    Nos paineis apresento os dashboards de produção de energia e outros indicadores de processos industriais.
                    Os dados foram coletados através do protocolo OPC DA, conectado ao software SCADA WinCC (Siemens).
                    Nesse projeto utilizei o Grafana para confecção dos painéis.
                </p>
                <ProjectImage
                    :src_img="require('@/assets/img/dash-energy.jpeg')"
                    :alt_img="'Graphs'"
                />
                <ProjectImage
                    :src_img="require('@/assets/img/dash-ind.jpeg')"
                    :alt_img="'Graphs'"
                />
                </div>
              </article>
        </dialog>
    </article>



</template>
<script>
import ProjectHead from '@/components/projects/ProjectHead.vue'
import ProjectImage from '@/components/projects/ProjectImage.vue'

export default {
    name:'DashBoard',
    components:{
        ProjectHead,
        ProjectImage
    },
    props:{
        title:String,
        subtitle:String,
        tag:String
    },
    methods:{
        open_modal: function (event) {
            const modal = document.getElementById(event.currentTarget.getAttribute("data-target"));
            modal.setAttribute("open", true);
        },
        close_modal:function (event){
            const modal = document.getElementById(event.currentTarget.getAttribute("data-target"));
            modal.removeAttribute("open");
        }
    }
}
</script>
<style scoped>
section{
  background-color: bisque;
  margin-top: 4em;
}
dialog article{
  width: 100%;
  max-width: 100%;
  height: 100%;
}

</style>