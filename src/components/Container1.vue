<template>
    <div class="container1">
        
        <div class="imageGallerie">
            <img src="../../src/assets/image_banner.avif" alt="Image banniere Openclassrooms">
        </div>
        <div class="becomeFutureProof">
            <h1><mark>&nbsp; Become &nbsp;<br />&nbsp; Future-Proof &nbsp; </mark></h1>
            <p>Get the skills of tomorrow</p>
            <p>Learn to learn efficiently</p>
            <p>Take control of your career for good</p>
            <button class="whiteButton"><a href="#">DISCOVER</a></button>
        </div>
        
    </div>
</template>

<script>
export default {
   name: 'displaycontainer1'
}
</script>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;500&display=swap');

.container1{
    font-family: 'Montserrat', sans-serif;
    display: flex;
    justify-content: center;
    background-color: #7451EB;
    height: 45vh;
    width: 100vw;
    color: white;
}

.container1 a {
    text-decoration: none;
}

.container1 p{
    margin: 0.5rem 0 0.5rem 0;
}

.becomeFutureProof{
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 25%;
}

.becomeFutureProof p {
    line-height: 0.5rem;
}

.imageGallerie img{
    height: 100%;
    margin-right: 2rem;
}

mark{
    color: white;
    background-color: #003668;
    
}

.whiteButton{
    background-color: white;
    padding: 0.5rem;
    font-family: 'Montserrat', sans-serif;
    font-weight: 700;
    color: #7451EB;
    font-weight: 800;
    border-radius: 5px;
    border-color: #7451EB;
    border-width: 1px;
    width: 10rem;
    height: 3rem;
    margin-top: 1rem;
}
.whiteButton:hover{
    box-shadow: rgba(0, 0, 0, 0.2) 0px 3px 1px -2px, rgba(0, 0, 0, 0.14) 0px 2px 2px 0px, rgba(0, 0, 0, 0.12) 0px 1px 5px 0px;
}

.whiteButton a {
    color: #7451EB;
}

@media screen and (max-width: 1200px){

    .becomeFutureProof{
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    }
    .container1{
        flex-direction: column;
        align-items: center;
        height: 100%;
    }

}

@media screen and (max-width: 1070px){
     .container1 .whiteButton{
       margin-bottom: 2rem;
    } 
}

@media screen and (max-width: 500px){
    .imageGallerie img {
        margin: 0;
        padding: 0;
        width: 100%;
    }
}
</style>