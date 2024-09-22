<script >
  export default {
	    data() {
	     return { 
			title: "We Boost Our Client's Bottom Line by Optimizing Their Growth Potential.",
            text: 'Quisque aliquet, libero consequat elementum convallis, erat risus imperdiet pellentesque sem neque eget.',
            img: '/img/we_boost/we-boost-our-clients.jpg',
            alt: '',
            button: 'Why Work With Us'
	      }
	   },
	 }
</script>

<template>

    <div class="container">
        <!-- titolo e descizione -->
        <div class="my-container text-center">
            <h2 class="fw-bold pb-5">
                {{ title }}
            </h2>
            <p>
                {{ text }}
            </p>
             <!-- bottone -->
            <button class="button orange-button mb-5">
                {{ button }}
            </button>

            <!-- immagine -->
            <div class="mb-3">
                <img :src="img" :alt="alt">
            </div>

        </div>
    </div>

</template>

<style lang="scss">
  @use 'src/assets/scss/partials/buttons.scss' as *;
  @use 'src/assets/scss/partials/variables.scss' as *;
  @use 'src/assets/scss/partials/page_main.scss' as *;
</style>