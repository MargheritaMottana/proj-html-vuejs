<script >

    import card from './Partials/card.vue';

  export default {
	    data() {
	     return { 
            title: 'Unlock Your Online Growth Potential',
            message: 'Online marketing to secure customer retention, leads, and sales. We focus on the bigger picture.',
            button: 'Our service',
	      }
	   },
       components:{
            card,
       }
	 }
</script>

<template>

    <div class="jumbotron">

        <div class="container">

            <div class="my-container">

                <div class="row">
                    <!-- titolo -->
                    <div class="col text-white">
                        <h1 class="fw-bold mb-3">
                            {{ title }}
                        </h1>
                        <p class="fs-5 mb-4">
                            {{ message }}
                        </p>
                        <button type="button" class="button white-button">
                            {{ button }} <i class="fa-solid fa-arrow-right ms-1"></i>
                        </button>
                    </div>

                    <!-- card -->
                    <div class="col d-flex justify-content-center">
                        <card/>
                    </div>
                </div>

            </div>

        </div>

    </div>
</template>

<style lang="scss">
  @use 'src/assets/scss/partials/page_jumbotron.scss' as *;
  @use 'src/assets/scss/partials/buttons.scss' as *;
  @use 'src/assets/scss/partials/variables.scss' as *;
</style>