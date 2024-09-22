<script >
  export default {
	    data() {
	     return { 
            paragraphs:[
                {
                    title: 'We Build Relationships',
                    text: 'Perspiciatis, modi nobis? Eaque modi similique libero possimus repellat perferendis id delectus.',
                },
                {
                    title: 'Proprietary Processes',
                    text: 'Perspiciatis, modi nobis? Eaque modi similique libero possimus repellat perferendis id delectus.',
                }
            ],
            icons:[
                {
                    img: '/img/main_icon/main_4_s2/image (2).png',
                    title: 'Accountability',
                    text: 'Curabitur ac leo nunc vestibulum',
                },
                {
                    img: '/img/main_icon/main_4_s2/image (3).png',
                    title: 'Transparency',
                    text: 'Curabitur ac leo nunc vestibulum',
                },
                {
                    img: '/img/main_icon/main_4_s2/image (4).png',
                    title: 'Investment',
                    text: 'Curabitur ac leo nunc vestibulum',
                },
            ]
	      }
	   },
	 }
</script>

<template>
        <div class="container pt-5">
            <div class="my-container">
                <div class="row align-items-center justify-content-between">

                    <!-- paragrafi -->
                    <div class="col-5">

                        <div v-for="(p, i) in paragraphs" :key="i" class="py-4">
                            <h3 class="pb-2">
                                {{ p.title }}
                            </h3>
                            <div>
                                {{ p.text }}
                            </div>
                        </div>

                    </div>
                    
                    <!-- icone + testo -->
                    <div class="col-6">

                        <div v-for="(icon, i) in icons" :key="i" class="d-flex align-items-center py-3">

                            <img :src="icon.img" :alt="icon.title" class="me-3">
                            <!-- testi -->
                            <div>
                                <h5 class="mb-3">
                                    {{ icon.title }}
                                </h5>
                                <div>
                                    {{ icon.text }}
                                </div>
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