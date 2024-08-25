<template>
    <section class="experience-section">
        <div class="container">
            <div class="intro has-text-centered">
                <p id="headingOne" class="is-size-4">
                    EXPERIENCE
                </p>
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
                { title: 'Job Title 1', description: 'Detailed description of what you did here1.' },
                { title: 'Job Title 2', description: 'Detailed description of what you did here2.' },
                { title: 'Job Title 3', description: 'Detailed description of what you did here3.' }
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
    width: 30%;
    background-color: #fff;
    padding: 10px;
    border-right: 2px solid #ddd;
}

.experience-item {
    padding: 10px;
    cursor: pointer;
    border-bottom: 1px solid #ddd;
    transition: background-color 0.3s;
}

.experience-item:hover {
    background-color: #007bff;
    color: #fff;
}

.experience-detail {
    width: 70%;
    padding: 20px;
    background-color: #fff;
}

.detail-content {
    display: none;
    padding: 10px;
    border: 1px solid #ddd;
    border-radius: 5px;
}

.detail-content.active {
    display: block;
}
</style>