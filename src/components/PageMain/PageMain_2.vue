<script >
  export default {
	    data() {
	     return { 
			title: 'Some Brands We Work With',
            text: 'Quisque aliquet, libero consequat elementum convallis.',
            brands: [
                {
                    img: '/img/loghi_brands/abstract.png',
                    alt: 'Abstract',
                },
                {
                    img: '/img/loghi_brands/cglobal.png',
                    alt: 'CGLOBAL',
                },
                {
                    img: '/img/loghi_brands/next.png',
                    alt: 'next',
                },
                {
                    img: '/img/loghi_brands/hemisferio.png',
                    alt: 'HEMISFERIO',
                },
                {
                    img: '/img/loghi_brands/spaces.png',
                    alt: 'spaces',
                },
                {
                    img: '/img/loghi_brands/digitalbox.png',
                    alt: 'digitalbox',
                },

            ],
            card:{
                img: '/img/experts/marketing-expert-cta.png',
                alt: 'Sandy Reiff',
                name:'Sandy Reiff',
                role: 'Marketing Consultant Expert',
                text: 'Drive Leads and Sales with Avada',
                button: '(555) 802-1234'
            }
	      }
	   },
	 }
</script>

<template>

    <div class="container">
        <!-- titolo e descizione -->
        <div class="my-container text-center">

            <h2 class="fw-bold pb-3">
                {{ title }}
            </h2>
            <p>
                {{ text }}
            </p>

            <div class="row">
                <!-- ciclo lettura dei brand -->
                <div class="col py-5" v-for="(brand, i) in brands" :key="i">
                    <img class="brands" :src="brand.img" :alt="brand.alt">
                </div>
            </div>

            <div class="cta-container row d-flex align-items-center shadow-lg rounded-4 py-2 px-5">

                <!-- foto - nome - ruolo -->
                <div class="col">
                    <div class="d-flex align-items-center">
                        <!-- foto -->
                        <img class="me-3 rounded-circle pro-pic-small" :src="card.img" :alt="card.alt">
                        <!-- testi -->
                        <div class="text-start">
                            <div class="fw-bold">
                                {{ card.name }}
                            </div>
                            <div class="font-small">
                                {{ card.role }}
                            </div>
                        </div>
                    </div>
                </div>
                <!-- cta -->
                <div class="col">
                    <div class="fw-bold">
                        {{ card.text }}
                    </div>
                </div>
                <!-- bottone numero -->
                <div class="col text-end">
                    <button class="button light-orange-button">
                        {{ card.button }}
                    </button>
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