<script lang="ts" setup>
  import ExperienceItem from './ExperienceItm.vue';
</script>

<template>
    <!-- ======= Resume Section ======= -->
    <section id="experience" class="resume">
      <div class="container" data-aos="fade-up">

        <div class="section-title">
          <h2>EXPERIENCE PROFESSIONEL</h2>
          <p>Magnam dolores commodi suscipit. Necessitatibus eius consequatur ex aliquid fuga eum quidem. Sit sint consectetur velit. Quisquam quos quisquam cupiditate. Et nemo qui impedit suscipit alias ea. Quia fugiat sit in iste officiis commodi quidem hic quas.</p>
        </div>

        <div class="row">
          <ExperienceItem
          poste="stage"
          date="MAI. 2023 – Août. 2023"
          company="CNAM"
          location="Paris, France"
          :desc="[
            'Conception et réalisation d‘une application mobile pour la Faculté des Sciences de Monastir (FSM).',
            'Conception et réalisation d’un site web pour le laboratoire Rlantis FSM.'
          ]"
          :tecno="['VueJs']"
          />
          <ExperienceItem
          poste="Projet de fin d’étude"
          date="janv. 2022 – Mai. 2022"
          company="RLANTIS FSM"
          location="Monastir, Tunisie"
          :desc="[
            'Conception et réalisation d‘une application mobile pour la Faculté des Sciences de Monastir (FSM).',
            'Conception et réalisation d’un site web pour le laboratoire Rlantis FSM.'
          ]"
          :tecno="['Flutter', 'Dart', 'Firebase', 'visual Studio code','PHP', 'Laravel', 'WampServer',
'Bootstrap']"
          />
          <ExperienceItem
          poste="Hackathon"
          date="janv. 2020 – fev. 2021"
          company="OpenGovDataHack 2020"
          location="Hammamet, Tunisie"
          :desc="['Application mobile pour la géolocalisation en temps réel des bus.']"
          :tecno="['Flutter', 'Dart', 'Firebase', 'visual Studio']"

          />

          <ExperienceItem
          poste="STAGE"
          date="juil. 2019 – aout. 2019"
          company="KOURA TECHNOLOGIE"
          location="Abidjan, Côte d’Ivoire"
          :desc="['Conception et réalisation d’application.']"
          :tecno="['progiciel Odoo']"
          />
        </div>
      </div>
    </section><!-- End Resume Section -->

</template>