<script >
  export default {
	    data() {
	     return { 
			title: 'Trusted by Leading Organisations',
            cards:[
                {
                    img: '/img/leading_organisations/case-studies-1.jpg',
                    alt: 'Spaces',
                    url: '#',
                    text: 'How SPaces attracted five millions visitors by improving the content',
                    data: '200%',
                    description: 'Higher revenue from digital',
                },
                {
                    img: '/img/leading_organisations/case-studies-4.jpg',
                    alt: 'Hemisferio',
                    url: '#',
                    text: 'Creativity helped Hemisferio to increase their brand reach vertically',
                    data: '10x',
                    description: 'Sales increase with the same ad spend',
                },
                {
                    img: '/img/leading_organisations/case-studies-6.jpg',
                    alt: 'DigitalBox',
                    url: '#',
                    text: 'How DigitalBox used AI-powered data insight to boost sales',
                    data: '3-year',
                    description: 'Partnership with Avada Consultant',
                }
            ],
            button: 'Read More Case Studies'
	      }
	   },
	 }
</script>

<template>

    <div class="container mb-5">
        <!-- titolo e descizione -->
        <div class="my-container text-center">
            <h2 class="fw-bold pb-5">
                {{ title }}
            </h2>

            <!-- cards -->
             <div class="row mb-5">
                <div class="col px-3" v-for="(card, i) in cards" :key="i">
                    <!-- immagine -->
                    <div class="mb-3 img-container">
                        <img :src="card.img" :alt="card.alt">
                        <a :href="card.url" class="gradient"></a>
                    </div>
                    <!-- testi -->
                    <div class="text-start">
                        <p :href="card.url" class="fs-5 mb-5">
                            {{ card.text }}
                        </p>
                        <h3 class="fw-bold">
                            {{ card.data }}
                        </h3>
                        <div class="font-small">
                            {{ card.description }}
                        </div>
                    </div>
                </div>
             </div>

             <!-- bottone -->
              <button class="button orange-button mb-5">
                {{ button }}
              </button>
        </div>
    </div>

</template>

<style lang="scss">
  @use 'src/assets/scss/partials/buttons.scss' as *;
  @use 'src/assets/scss/partials/variables.scss' as *;
  @use 'src/assets/scss/partials/page_main.scss' as *;
</style>