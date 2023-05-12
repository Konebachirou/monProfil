<script>
    export default{
        data() {
        return {
            isHome: false,
            isAbout: false,
            isSkills: false,
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

        goToSkills() {
            this.changeNavigationState("skill")
        },

        

        changeNavigationState(destination) {
            this.isAbout = false
            this.isHome = false
            this.isSkills = false

            switch (destination) {
                case "home":
                    this.isHome = true
                    break;
                case "about":
                    this.isAbout = true
                    break;
                case "skill":
                    this.isSkills = true
                    break;

                default:
                    this.isHome = true
                    break;
            }
        }
    }
    }
</script>