<script>
    import Section_1 from './PageMain_4_sections/Section_1.vue';
    import Section_2 from './PageMain_4_sections/Section_2.vue';
    import Section_3 from './PageMain_4_sections/Section_3.vue';

    export default {
        data() {
            return { 
            }
        },
        components:{
            Section_1,
            Section_2,
            Section_3,
        }
        }
</script>

<template>

    <!-- Create le sotto sezioni per inserirle tutte all'interno dello sfondo con gradiente -->

    <div class="bg-gray-gradient pt-5 pb-5">
        <Section_1/>
        <Section_2/>
        <Section_3/>
    </div>

</template>

<style lang="scss">
  @use 'src/assets/scss/partials/buttons.scss' as *;
  @use 'src/assets/scss/partials/variables.scss' as *;
  @use 'src/assets/scss/partials/page_main.scss' as *;
</style>