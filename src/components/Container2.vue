<template>
     <div class="container2">

         <displayElementContainer2 :data="cards[0]" />
         <displayElementContainer2 :data="cards[1]"/>
         <displayElementContainer2 :data="cards[2]"/>
    
    </div>
</template>

<script>

import displayElementContainer2 from './elementContainer2.vue'

export default {
    name: 'displayTheContainer2',
    data() {
        return {
            cards: [
                {
                    src: "diploma.svg", 
                    title: "Diploma Qualification",
                    description: "Earn a bachelor's or master's-level diploma to unlock your new career"
                },
                 {
                    src: "../../src/assets/mentorship.svg",
                    title: "Mentorship",
                    description: "Benefit from weekly one-to-one sessions with an expert in the target profession"
                },
                 {
                    src: "../../src/assets/job.svg",
                    title: "Job",
                    description: "Find a job within 6 months or we guarantee the reimbursement of your tution*"
                },
            ]
        }
    },
    components: {
        displayElementContainer2
    }
}
</script>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;500&display=swap');


.container2{
display: flex;
justify-content: center;
margin-top: 5rem;
}

.container2 h2{
    text-align: center;
    color: #003668;
    font-weight: 700;
    font-size: 1rem;
}

.container2 p{
    text-align: center;
    font-weight: 400;
    font-size: 0.8rem;
}

.container2 img{
    margin: 0 5rem 0 5rem;
}

@media screen and (max-width: 1200px){
    .container2{
        flex-direction: column;
        align-items: center;
    }
}

@media screen and (max-width: 1070px){
    .container2{
        margin-top: 2rem;
    }

    .container2 img {
        width: 100%;
        margin: 0;
    }

    .container2 h2{
        font-size: 2rem;
    }

    .container2 p{
        font-size: 1rem;
        margin-bottom: 4rem;
    }

    .diplomaQualification, .Mentorship, .Job{
        width: 40%;
        font-size: 2rem;
    } 
}

@media screen and (max-width: 500px){
    .container2 h2{
        font-size: 2rem;
    }

    .container2 p{
        font-size: 1rem;
        margin-bottom: 4rem;
    }

    .diplomaQualification, .Mentorship, .Job{
        width: 60%;
        font-size: 2rem;
    } 

}

</style>