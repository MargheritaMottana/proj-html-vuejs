<script >
  export default {
	    data() {
	     return { 
			title: "We Boost Our Client's Bottom Line by Optimizing Their Growth Potential.",
            text: 'Quisque aliquet, libero consequat elementum convallis, erat risus imperdiet pellentesque sem neque eget.',
            img: '/img/we_boost/we-boost-our-clients.jpg',
            alt: "We Boost Our Client",
            button: 'Why Work With Us'
	      }
	   },
	 }
</script>

<template>
     <div class="my-container pt-5">
        <div class="container">

            <div class="row align-items-center justify-content-between">

                <!-- testi + bottone -->
                <div class="col-5">
                    <h2 class="fw-bold pb-3">
                        {{ title }}
                    </h2>
                    <p class="pb-3">
                        {{ text }}
                    </p>
                    <button class="button orange-button mb-5">
                        {{ button }}
                    </button>
                </div>
                
                <!-- immagine -->
                <div class="col-6">
                    <img class="rounded-3 shadow" :src="img" :alt="alt">
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