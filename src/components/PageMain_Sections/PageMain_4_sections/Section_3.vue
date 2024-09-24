<script >
  export default {
	    data() {
	     return { 
            title: 'Awards',
            icons:[
                {
                    img: '/img/main_icon/main_4_s3/award-a.png',
                    title: 'award',
                    text: 'Winner Seo Master MAGT Smart Start Award 2017',
                },
                {
                    img: '/img/main_icon/main_4_s3/award-b.png',
                    title: 'award',
                    text: 'Top Social Media Agencies Next Partner 2018',
                },
                {
                    img: '/img/main_icon/main_4_s3/award-c.png',
                    title: 'award',
                    text: '10 Fastest Growing Abstract Solution Providers 2019',
                },
                {
                    img: '/img/main_icon/main_4_s3/award-d.png',
                    title: 'award',
                    text: 'National Excellence Agencie Award Winner 2020',
                },
            ]
	      }
	   },
	 }
</script>

<template>
    <div class="my-container py-5">
        <div class="container text-center">

            <!-- titolo sezione -->
            <h3 class="pb-3">
                {{ title }}
            </h3>

            <!-- icone + testo -->
            <div class="row justify-content-between">
                
                <!-- ciclo per lettura di tutti i loghi -->
                <div class="col" v-for="(icon, i) in icons" :key="i">

                    <!-- in css cambio di colore con i filtri -->
                    <img :src="icon.img" :alt="icon.title" class="award">
                    <div>
                        {{ icon.text }}
                    </div>

                </div>

            </div>

        </div>
    </div>
</template>

<style lang="scss">
  @use 'src/assets/scss/partials/buttons.scss' as *;
  @use 'src/assets/scss/partials/variables.scss' as *;
  @use 'src/assets/scss/partials/page_main.scss' as *;
</style>