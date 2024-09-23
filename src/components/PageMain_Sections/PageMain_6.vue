<script >
  export default {
	    data() {
	     return { 
			title: 'Marketing Resources: Insider Advice on How to Increase Online Sales',
            button: 'Explore All Resources',
            cards:[
                {
                    img: '/img/marketing_resources/blog-posts-6.jpg',
                    alt: 'Marketing Tips',
                    url: '#',
                    text: 'Marketing Tips And Tricks For Your Website',
                },
                {
                    img: '/img/marketing_resources/blog-posts-5.jpg',
                    alt: 'Write Stunning Blog',
                    url: '#',
                    text: 'How to Write Stunning Blog Post Titles',
                },
                {
                    img: '/img/marketing_resources/blog-posts-4.jpg',
                    alt: 'Reduce Facebook Ads Spend',
                    url: '#',
                    text: 'Techniques to Reduce Facebook Ads Spend',
                }
            ],
	      }
	   },
	 }
</script>

<template>
    <div class="bg-gray-gradient pt-5 pb-5">

        <div class="container mb-5">

            <div class="my-container">

                 <!-- titolo e bottone-->
                <div class="row">

                    <!-- titolo -->
                    <h2 class="col-5 fw-bold pb-5">
                        {{ title }}
                    </h2>
                    <!-- bottone -->
                     <div class="col text-end align-self-end">
                        <button class="button orange-button mb-5">
                             {{ button }}
                        </button>
                     </div>

                </div>

                <!-- cards -->
                <div class="row mb-5">
                    <div class="col" v-for="(card, i) in cards" :key="i">
                        <!-- immagine -->
                        <div class="mb-3 img-container">
                            <img :src="card.img" :alt="card.alt" class="">
                            <a :href="card.url" class="gradient"></a>
                        </div>
                        <!-- testi -->
                        <div class="text-start">
                            <p :href="card.url" class="fs-5 mb-5">
                                {{ card.text }}
                            </p>
                        </div>
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