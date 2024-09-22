<script >
  export default {
	    data() {
	     return { 
            img: '/img/testimonial/large-testimonial.jpg',
            alt: 'Kate Schadler',
            quote: '"The team at Avada Marketing Consultant is fabulous. They helped us unlock our potential online and offline. We have experienced year on year growth due to their progressive approach."',
            name: 'Kate Schadler',
            role: 'Marketing Consultant - Abstract'
	      }
	   },
	 }
</script>

<template>
        <div class="container pt-5">
            <div class="my-container py-5">
                <div class="row align-items-center justify-content-between">

                    <!-- immagine -->
                    <div class="col-6">
                        <img class="rounded-3" :src="img" :alt="alt">
                    </div>

                    <!-- testi -->
                    <div class="col-5">
                        <h3 class="pb-4">
                            {{ quote }}
                        </h3>
                        <div class="fw-bold mb-1">
                            {{ name }}
                        </div>
                        <p class="font-small">
                            {{ role }}
                        </p>
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