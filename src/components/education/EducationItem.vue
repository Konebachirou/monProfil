<script setup>

defineProps({
  title: {type: String, required: true},
  date: {type: String, required: true},
  school: {type: String, required: true},
  location: {type: String, required: true}
 });

   
</script>

<template>
    <div class="col-md-6">
        <div class="resume-item">
            <h4>{{title}}</h4>
            <h5>{{ date }}</h5>
            <p><em>{{ location }}</em></p>
            <p>{{school}}</p>
        </div>
    </div>
</template>

<style scoped>
.resume-item {
  padding: 0 0 20px 20px;
  margin-top: -2px;
  border-left: 2px solid #0563bb;
  position: relative;
}

.resume-item h4 {
  line-height: 18px;
  font-size: 18px;
  font-weight: 600;
  text-transform: uppercase;
  font-family: "Poppins", sans-serif;
  color: #0563bb;
  margin-bottom: 10px;
}

.resume-item h5 {
  font-size: 16px;
  background: #f7f8f9;
  padding: 5px 15px;
  display: inline-block;
  font-weight: 600;
  margin-bottom: 10px;
}
.resume-item:last-child {
  padding-bottom: 0;
}

.resume-item::before {
  content: "";
  position: absolute;
  width: 16px;
  height: 16px;
  border-radius: 50px;
  left: -9px;
  top: 0;
  background: #fff;
  border: 2px solid #0563bb;

  margin-bottom: 20px;
}
</style>