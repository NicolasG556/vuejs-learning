<template>
    <div class="navbarContainer" id="navbarMenu">
        <div id="closeNav"><img src="../../src/assets/close.png" alt="closeButton"></div>
        <ul class="navbar">
            <li><a href="#"><img class="logoOpenclassroom" src="../../src/assets/logo.png" alt="logo Openclassrooms"></a></li>
            <li><a href="#">Training programs <span class="iconFlecheVersLeBas">▼</span></a></li>
            <li><a href="#">Apprenticeship</a></li>
            <li><a href="#">Funding options</a></li>
            <div class="pipeSeparation">|</div>
            <li><a href="#">For Business</a></li>
        </ul>
        <ul class="navbar2">
            <li class="logoResearch"><a href="#"><img src="../../src/assets/magnifying-glass.png" alt="logo research" width="25rem"></a></li>
            <li><button class="navbarButton"><a href="#">SIGN IN</a></button></li>
          </ul>
    </div>
</template>

<script>
export default {
    name: 'displayNavbar'
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;500&display=swap');



.navbarContainer{
    font-family: 'Montserrat', sans-serif;
    height: 4rem;
    display: flex;
    justify-content: center;
}

#closeNav{
    position: absolute;
    width: 1.5rem;
    top: 0;
    right: 0;
    margin: 1rem 1rem 0 0;
}

#closeNav img{
    width: 100%;
}

.navbar{
    display: flex;
    justify-content: center;
    align-content: space-around;
    align-items: center;
    list-style-type: none;
    height: 4rem;
    margin: 0 2rem 0 4rem;
    padding: 0 2rem 0 2rem; 
}

.navbar2{
    display: flex;
    justify-content: center;
    align-content: space-around;
    align-items: center;
    list-style-type: none;
    height: 4rem;
    margin: 0 3rem 0 2rem;
    padding: 0 2rem 0 2rem; 
}

.navbar li{
    margin: 1.5rem;
}

.navbar a {
    text-decoration: none;  
    color: black;
    font-size: 0.8rem;
}

.navbar2 a{
    text-decoration: none;  
    color: black;
    font-size: 0.8rem;
}

.navbar2 li{
    margin: 0.5rem;
}

.logoResearch img:hover{
    color: #7451EB;
}

.pipeSeparation{
    font-size: 1.5rem;
    color: #E0E0E0
}

.iconFlecheVersLeBas{
    font-size: 0.6rem;
}

.logoOpenclassroom{
    width: 20em;
}
.navbarButton{
    background-color: white;
    padding: 0.5rem;
    font-family: 'Montserrat', sans-serif;
    font-weight: 700;
    color: #7451EB;
    font-weight: 800;
    border-radius: 5px;
    border-color: #7451EB;
    border-width: 1px;
}

.navbarButton:hover{
    background-color: #DED5FA;
}

.navbarButton a {
    color: #7451EB;
}

@media screen and (max-width: 1400px){

    .navbar{
        margin: 0;
    }

    .navbar2{
        margin: 0;
    }
}

@media screen and (max-width: 1200px){
    .navbar{
        padding: 0;
    }

    .navbar2{
        padding: 0;
    }
}

@media screen and (max-width: 1070px){
    .navbarContainer{
        flex-direction: column;
        height: 100vh;
        width: 60vw;
        margin-bottom: 2rem;
        position: fixed;
        background-color: white;
        box-shadow:  rgba(0, 0, 0, 0.2) 0px 5px 1px -2px, rgba(0, 0, 0, 0.14) 0px 4px 2px 0px, rgba(0, 0, 0, 0.12) 0px 3px 5px 0px;;
    }

     .navbarContainer a{
        font-size: 1rem;
    }

    .navbar{
        height: 100%;    
        width: 100%;
        flex-direction: column;
    }

    .closedNavbar{
        transform: translate(-100%);
        height: 0;
    }

    .navbar a{
        font-size: 1.5rem;
    }

    .navbar2{
        height: 20%;
        width: 100%;
        align-self: center;
    }

    .logoOpenclassroom{
        width: 100%;
    }

    .navbar2 a {
        font-size: 1.5rem;
    }
}

@media screen and (max-width: 500px){
    .navbar a{
        font-size: 1rem;
    }
}

@media screen and (max-width: 430px){
      .navbarContainer{
        flex-direction: column;
    }

    .navbar, .navbar2{
        width: 100%;
    }
}

</style>