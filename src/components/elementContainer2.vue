<template>

    <section>
        <div class="diplomaQualification">
            <img :src= "data.src" />
            <h2>{{ data.title }}</h2>
            <p>{{ data.description }}</p>
        </div>
    </section>

</template>

<script>
export default {
    name : 'displayElementContainer2',
    props: {
       data: Object
    }
}


</script>

<style scoped>
    section{
        width: 20rem;
        margin: 0 5rem 0 5rem
    }
</style>