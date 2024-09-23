<script >

    import card from '../Partials/card.vue';

  export default {
	    data() {
	     return { 
            title: "Let's Make Things Happen",
            text: 'Curabitur ac leo nunc. Vestibulum et mauris vel ente finibus maximum nec ut leo. Integer consectetur.',
            quote: '"The team at Avada Marketing Consultant is fabulous. They helped us unlock our potential online and offline. We have experienced year on year growth due to their progressive approach."',
            name: 'George Anderson',
            role: 'DigitalBox CEO',
	      }
	   },
       components:{
        card,
       }
	 }
</script>

<template>

    <footer class="bg-black">

        <div class="container">

            <div class="my-container">

                <div class="row">

                    <div class="col text-white">

                        <!-- titolo e testo -->
                        <h1 class="fw-bold mb-4">
                            {{ title }}
                        </h1>
                        <p class="fs-5 mb-5">
                            {{ text }}
                        </p>

                        <!-- suddivisione per citazione -->
                        <hr class="mb-5">
                        <p class="fst-italic mb-4">
                            {{ quote }}
                        </p>
                        <div class="fw-bold mb-2">
                            {{ name }}
                        </div>
                        <p class="font-small">
                            {{ role }}
                        </p>

                    </div>

                    <!-- card -->
                    <div class="col d-flex justify-content-center">
                        <card/>
                    </div>

                </div>

            </div>

        </div>

    </footer>
</template>

<style lang="scss">
  @use 'src/assets/scss/partials/page_footer.scss' as *;
  @use 'src/assets/scss/partials/buttons.scss' as *;
  @use 'src/assets/scss/partials/variables.scss' as *;
</style>