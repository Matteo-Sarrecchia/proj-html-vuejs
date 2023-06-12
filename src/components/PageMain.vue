<script>
import FounderCeoSection from './FounderCeoSection.vue'


export default {
    name: "PageMain",
    components: {
        FounderCeoSection
    }
}
</script>

<template>
    <main>
        <FounderCeoSection />
    </main>
</template>

<style lang="scss" scoped>
@use "../styles/generals.scss" as *;

main {
    border: 1px solid black;
    min-height: 300px;
}
</style>
