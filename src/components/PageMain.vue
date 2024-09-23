<script>
    import PageMain_1 from './PageMain_Sections/PageMain_1.vue';
    import PageMain_2 from './PageMain_Sections/PageMain_2.vue';
    import PageMain_3 from './PageMain_Sections/PageMain_3.vue';
    import PageMain_4 from './PageMain_Sections/PageMain_4.vue';
    import PageMain_5 from './PageMain_Sections/PageMain_5.vue';
    import PageMain_6 from './PageMain_Sections/PageMain_6.vue';

    export default {
        data() {
            return { 
            }
        },
        components:{
            PageMain_1,
            PageMain_2,
            PageMain_3,
            PageMain_4,
            PageMain_5,
            PageMain_6,
        }
    }
</script>

<template>

    <div>
        <PageMain_1/>
        <PageMain_2/>
        <PageMain_3/>
        <PageMain_4/>
        <PageMain_5/>
        <PageMain_6/>
    </div>

</template>

<style lang="scss">
  @use 'src/assets/scss/partials/buttons.scss' as *;
  @use 'src/assets/scss/partials/variables.scss' as *;
  @use 'src/assets/scss/partials/page_main.scss' as *;
</style>