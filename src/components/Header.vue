<script >
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

    mounted(){
        this.changeNavigationState("home");
    },

    methods: {
        goToHome() {
            this.changeNavigationState("home")
        },
        goToAbout() {
            this.changeNavigationState("about")
        },

        goToEducation() {
            this.changeNavigationState("education")
        },
        goToExperience() {
            this.changeNavigationState("experience")
        },
        goToSkills() {
            this.changeNavigationState("skill")
        },
        goToProject() {
            this.changeNavigationState("project")
        },
        goToContact() {
            this.changeNavigationState("contact")
        },
        
        changeNavigationState(destination) {
            this.isAbout = false
            this.isHome = false
            this.isSkills = false
            this.isEducation= false
            this.isExperience= false
            this.isProject= false
            this.isContact= false

            switch (destination) {
                case "home":
                    this.isHome = true
                    break;
                case "about":
                    this.isAbout = true
                    break;
                case "education":
                    this.isEducation = true
                    break;
                case "experience":
                    this.isExperience = true
                    break;
                case "skill":
                    this.isSkills = true
                    break;
                case "project":
                    this.isProject = true
                    break;
                case "contact":
                    this.isContact = true
                    break;

                default:
                    this.isHome = true
                    break;
            }
        }
    }
    }

     /**
   * Easy selector helper function
   */
  const select = (el, all = false) => {
    el = el.trim()
    if (all) {
      return [...document.querySelectorAll(el)]
    } else {
      return document.querySelector(el)
    }
  }

</script>

<template>
  <i class="bi bi-list mobile-nav-toggle d-lg-none"></i>
  <header id="header" class="d-flex flex-column justify-content-center">
    <nav id="navbar" class="navbar nav-menu">
      <ul>
        <!-- <Item lien="#hero"/> -->
        <li><a href="#hero" class="nav-link scrollto " :class="{ active: isHome }" @click="goToHome()"><i class="bx bx-home"></i> <span>Home</span></a></li>
        <li><a href="#about" class="nav-link scrollto" :class="{ active: isAbout }" @click="goToAbout()"><i class="bx bx-user"></i> <span>About</span></a></li>
        <li><a href="#education" class="nav-link scrollto" :class="{ active: isEducation }" @click="goToEducation()"><i class='bx bxs-graduation'></i> <span>Education</span></a></li>
        <li><a href="#experience" class="nav-link scrollto" :class="{ active: isExperience }" @click="goToExperience()"><i class='bx bx-briefcase'></i> <span>Experience</span></a></li>
        <li><a href="#skills" class="nav-link scrollto" :class="{ active: isSkills }" @click="goToSkills()"> <i class="bx bx-hive"></i><span>Skills</span></a></li>
        <li><a href="#project" class="nav-link scrollto" :class="{ active: isProject }" @click="goToProject()"> <i class='bx bx-task'></i><span>Project</span></a></li>
        <li><a href="#contact" class="nav-link scrollto" :class="{ active: isContact }" @click="goToContact()"><i class="bx bx-envelope" ></i> <span>Contact</span></a></li>
      </ul>
    </nav><!-- .nav-menu -->
  </header><!-- End Header -->
</template>