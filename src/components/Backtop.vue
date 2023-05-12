<script>
    export default{
        data() {
        return {
            isHome: false,
            isAbout: false,
            isSkills: false,
            isEducation: false,
            isExperience: false,
            isProject: false,
            isContact: false,
        }
    },

    methods:{
        getScroll(){
    console.log(window.scrollBy)

        }
    }
 }

</script>



<template>
    <a href="#" class="back-to-top d-flex align-items-center justify-content-center active " @click.prevent="getScroll()"><i class="bi bi-arrow-up-short"></i></a>
</template>
<style scoped>
    .back-to-top {
  position: fixed;
  visibility: visible;
  opacity: 0;
  right: 15px;
  bottom: 15px;
  z-index: 996;
  background: #0563bb;
  width: 40px;
  height: 40px;
  border-radius: 50px;
  transition: all 0.4s;
}

.back-to-top i {
  font-size: 28px;
  color: #fff;
  line-height: 0;
}

.back-to-top:hover {
  background: #0678e3;
  color: #fff;
}

.back-to-top.active {
  visibility: visible;
  opacity: 1;
}
</style>
