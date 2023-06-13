<script>
import FounderCeoSection from './FounderCeoSection.vue'
import ServicesSection from './ServicesSection.vue'
import CoursesSection from './CoursesSection.vue'




export default {
    name: "PageMain",
    components: {
        FounderCeoSection,
        ServicesSection,
        CoursesSection
    }
}
</script>

<template>
    <main>
        <FounderCeoSection />
        <ServicesSection />
        <CoursesSection />
    </main>
</template>

<style lang="scss" scoped>
@use "../styles/generals.scss" as *;

main {
    border: 1px solid black;
    min-height: 300px;
}
</style>
