
<script lang="ts" setup>
  import EducationItem from './EducationItem.vue';
</script>

<template>
    <section id="education">
      <div class="container"  data-aos="fade-up">

        <div class="section-title">
          <h2>Education</h2>
          <p>Magnam dolores commodi suscipit. Necessitatibus eius consequatur ex aliquid fuga eum quidem. Sit sint consectetur velit. Quisquam quos quisquam cupiditate. Et nemo qui impedit suscipit alias ea. Quia fugiat sit in iste officiis commodi quidem hic quas.</p>
        </div>

        <div class="row">
         
           <EducationItem  
            title="Master 2  en Methodes Informatique Appliqués a la Gestion d'Entreprise (MIAGE)"
            date="2010 - 2014"
            location="Portland par 127,Orlando, FL"
            school="Université evry"
            />

            <EducationItem  
            title="Licence en Génie Logiciel & Système d'Information (LGLSI)"
            date="2019 - 2022"
            location="Monastir, Tunisie"
            school="Faculté des Sciences de Monastir (FSM)"
            />
            <EducationItem  
            title="LICENCE 1 en Methodes Informatique Appliqués a la Gestion d'Entreprise (MIAGE) "
            date="2018 - 2019"
            location="Bingerville, Côte d’Ivoire"
            school="Université Polytechnique de Bingerville"
            />
            <EducationItem  
            title="BACCALAUREAT SCIENTIFIQUE (SERIE C)"
            date="2017 - 2018"
            location="Grand-Bassam, Côte d’Ivoire"
            school="Lycée Moderne 1 de Grand-Bassam"
            />

        </div>
      </div>
    </section><!-- End Resume Section -->

</template>
