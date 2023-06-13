<script>
import FounderCeoSection from './FounderCeoSection.vue'
import ServicesSection from './ServicesSection.vue'
import CoursesSection from './CoursesSection.vue'
import TalkAboutSection from './TalkAboutSection.vue'
import BlogSection from './BlogSection.vue'

export default {
    name: "PageMain",
    components: {
        FounderCeoSection,
        ServicesSection,
        CoursesSection,
        TalkAboutSection,
        BlogSection
    }
}
</script>

<template>
    <main>
        <FounderCeoSection />
        <ServicesSection />
        <CoursesSection />
        <TalkAboutSection />
        <BlogSection />
    </main>
</template>

<style lang="scss" scoped>
@use "../styles/generals.scss" as *;

main {
    border: 1px solid black;
    min-height: 300px;
}
</style>
