<script >
  export default {
	    data() {
	     return { 
			contents: [
				{
					image : '/img/svg/img1.svg',
					icon: '/img/main_icon/icona1.png',
					scope : 'Business Growth',
					title : 'Increase Brand Awareness',
					text : 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla dignissimos assumenda, laboriosam iusto in nisi eos repudiandae ullam!',
					button : 'Get a Consultation'
				},
				{
					image : '/img/svg/img2.svg',
					icon: '/img/main_icon/icona2.png',
					scope : 'Investors In People',
					title : 'In-House Sales Training',
					text : 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla dignissimos assumenda, laboriosam iusto in nisi eos repudiandae ullam!',
					button : 'Get a Consultation'
				},
				{
					image : '/img/svg/img3.svg',
					icon: '/img/main_icon/icona3.png',
					scope : 'Social Media Analysis',
					title : 'Harness Your Social Proof',
					text : 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla dignissimos assumenda, laboriosam iusto in nisi eos repudiandae ullam!',
					button : 'Get a Consultation'
				},
				
			],
	      }
	   },
	 }
</script>

<template>

    <div class="container">
		<div class="my-container">

			<section class="row align-items-center justify-content-between content" v-for="(content, i) in contents" :key="i">

				<!-- imagine -->
				<div class="col">
					<img :src="content.image" :alt="content.title" class="content-img">
				</div>
				
				<!-- testo -->
				<div class="col-5">
					<!-- scopo -->
					<div class="d-flex align-items-center mb-3">
						<div>
							<img :src="content.icon" :alt="content.scope" class="scope-img me-3">
						</div>
						<div>
							{{ content.scope }}
						</div>
					</div>
					<!-- titolo -->
					<h2 class="fw-bold mb-4">
						{{ content.title }}
					</h2>
					<!-- testo e cta -->
					<p class="mb-4">
						{{ content.text }}
					</p>
					<button type="button" class="button orange-button">
                    	{{ content.button }}
                	</button>
				</div>

			</section>

		</div>
    </div>
    
</template>

<style lang="scss">
  @use 'src/assets/scss/partials/buttons.scss' as *;
  @use 'src/assets/scss/partials/variables.scss' as *;
  @use 'src/assets/scss/partials/page_main.scss' as *;
</style>