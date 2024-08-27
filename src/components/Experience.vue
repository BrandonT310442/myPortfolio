<template>
    <section class="experience-section">
        <div class="container">
            <div class="intro has-text-centered">
                <p id="headingOne" class="is-size-4">
                    EXPERIENCE
                </p>
                <br>
            </div>
            <div class="experience-container">
                <div class="experience-list">
                    <div v-for="(item, index) in experienceItems" :key="index" class="experience-item"
                        :data-detail="index + 1" @click="showDetail(index + 1)">
                        {{ item.title }}
                    </div>
                </div>
                <div class="experience-detail">
                    <div v-for="(item, index) in experienceItems" :key="index" :id="'detail-' + (index + 1)"
                        class="detail-content" :class="{ active: activeDetail === index + 1 }">
                        <h3 class="title is-size-5">{{ item.title }}</h3>
                        <p>{{ item.description }}</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            activeDetail: 1, // Set default to show Job 1's description
            experienceItems: [
                { title: 'Supply Chain Management Intern', description: "Helped create and analyze BOM's with Microsoft Excel, streamlining data management and improving procurement efficiency. Performed routine warehouse inventory audits to ensure accurate purchasing from each supplier, optimizing parts procurement and minimizing excess stock. Gained hands-on experience with circuit boards and engineering drawings, actively contributing to tasks in the server room." },
                { title: 'Lead Software Developer, FIRST Robotics Competition Team 7558', description: 'Helped train over 30 team members for effective match scouting. Developed a scouting app using the MEVN stack for effective game analysis for alliance selection. Achieved over a 72% win rate and First Place in the Galileo Division at the FRC World Championships.' },

                { title: 'Head of Media on Student Executive Council ', description: 'Responsible for full-year assembly video production for assemblies and entertainment, along with photography at events that were led by the Student Council. Managed events such as Semi-Formal Dance and Spirit Days.' },
            ]
        };
    },
    methods: {
        showDetail(index) {
            this.activeDetail = index;
        }
    }
};
</script>

<style scoped>
#headingOne {
    color: #007bff;
    font-family: "Work Sans", sans-serif;
    font-weight: 600;
    letter-spacing: .2rem;
    text-decoration: underline;
    text-underline-offset: 10px;
}

.experience-section {
    padding: 20px;
}

.experience-container {
    display: flex;
}

.experience-list {
    font-family: "Work Sans", sans-serif;
    font-weight: 600;
    letter-spacing: 0.2rem;
    color: #007bff;
    width: 40%;
    background-color: #fff;
    padding: 10px;
    border-right: 2px solid #ddd;
    text-transform: uppercase;
}

.experience-item {
    padding: 10px;
    cursor: pointer;
    border-bottom: 1px solid hsl(0, 0%, 87%);
    transition: 0.2s ease-in;
}

.experience-item:hover {
    opacity: 0.5;
    transition: 0.2s ease-out;
    text-underline-offset: 10px;
}

.experience-detail {
    width: 70%;
    padding: 20px;
    background-color: #fff;
}

.detail-content {
    opacity: 0;
    max-height: 0;
    overflow: hidden;
    transition: opacity 0.3s ease, max-height 0.3s ease;
}

.detail-content.active {
    opacity: 1;
    max-height: 1000px;
    /* Arbitrary large value to accommodate content */
}

.fade-enter-active,
.fade-leave-active {
    transition: opacity 0.5s, max-height 0.5s;
}

.fade-enter,
.fade-leave-to {
    opacity: 0;
    max-height: 0;
}

.title {
    color: #007bff;
    text-transform: uppercase;
    font-weight: normal
}
</style>
