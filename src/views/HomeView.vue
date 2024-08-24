<script setup>
import Intro from '../components/Intro.vue';
import Skills from '../components/Skills.vue';
import Projects from '../components/Projects.vue';
import OtherProjects from '@/components/OtherProjects.vue';
</script>

<template>
    <Intro class="fade-in" />
    <Skills class="fade-in" />
    <Projects class="fade-in" />
    <OtherProjects class="fade-in" />>
</template>

<style scoped>
.fade-in {
    opacity: 0;
    animation: fadeIn 3.5s forwards;
}

@keyframes fadeIn {
    from {
        opacity: 0;
    }

    to {
        opacity: 1;
    }
}
</style>
