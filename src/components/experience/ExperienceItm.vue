<script setup>

defineProps({
  poste: {type: String, required: true},
  date: {type: String, required: true},
  company: {type: String, required: true},
  location: {type: String, required: true},
  desc: {type: Array,  },
  tecno: {type: Array,  }
 });

   
</script>

<template>
        <div class="col-lg-6">
            <div class="resume-item">
              <h4>{{poste}}</h4>
              <h5>{{date}}</h5>
              <p><em>{{location}}</em></p>
              <ul>
                <li v-for="item in desc">
                    {{ item }}
                </li>
                <h5>Outils utilisés : </h5>
              <span class="tecno" v-for="item in tecno">{{ item }}</span>
              </ul>
            </div>
    </div>
</template>


<style scoped>

.resume-title {
  font-size: 26px;
  font-weight: 700;
  margin-top: 20px;
  margin-bottom: 20px;
  color: #45505b;
}
.resume-item {
  padding: 0 0 20px 20px;
  margin-top: -2px;
  border-left: 2px solid #0563bb;
  position: relative;
}
.resume .resume-item ul {
  padding-left: 20px;
}

.resume .resume-item ul li {
  padding-bottom: 10px;
}

.resume .resume-item ul li h5 {
  color: #0563bb;
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

.resume-item .tecno{
  font-size: 14px;
  padding: 8px;
  background: #0563bb;
  color: #fff;
  border-radius: 50px;
  display: inline-flex;
  align-items: center;
  margin: 1%;
  justify-content: center;
}
</style>