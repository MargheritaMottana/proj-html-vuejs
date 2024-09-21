<script >
  export default {
	    data() {
	     return { 
			title: 'Trusted by Leading Organisations'
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
        </div>
    </div>

</template>

<style lang="scss">
  @use 'src/assets/scss/partials/buttons.scss' as *;
  @use 'src/assets/scss/partials/variables.scss' as *;
  @use 'src/assets/scss/partials/page_main.scss' as *;
</style>