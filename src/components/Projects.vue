<template>
    <div class="intro">
        <p id="headingOne" class="is-size-4">FEATURED PROJECTS</p>

        <!-- Vortex AI -->
        <div class="columns is-vcentered">
            <!-- Image Section -->
            <div class="column is-three-quarters">
                <img id="vortexAI" src="../assets/VortexAIbg2.png" alt="Vortex AI">
            </div>

            <!-- Text Section -->
            <div class="column">
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae est culpa, laborum sint autem corrupti
                    voluptas, ipsum id ab eveniet ea atque deleniti accusamus et, alias temporibus modi aspernatur
                    impedit.</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {}
</script>

<style scoped>
/* Styling for the heading */
#headingOne {
    color: #007bff;
    font-family: "Work Sans", sans-serif;
    font-weight: 600;
    letter-spacing: 0.2rem;
    text-decoration: underline;
    text-underline-offset: 10px;
    margin-top: 100px;
    margin-right: 50px;
    z-index: 1.0;
    transform: translateX(10%);
}

/* Image Size */
#vortexAI {
    margin-top: 15px;
    margin-left: 100px;
    width: 666.66px;
    height: 471.333px;
}
</style>