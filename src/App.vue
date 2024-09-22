<script >
	import PageHeader from './components/PageHeader.vue';
	import PageMain_1 from './components/PageMain/PageMain_1.vue';
	import PageMain_2 from './components/PageMain/PageMain_2.vue';
	import PageMain_3 from './components/PageMain/PageMain_3.vue';
	import PageMain_4 from './components/PageMain/PageMain_4.vue';
	import PageMain_5 from './components/PageMain/PageMain_5.vue';
	import PageFooter from './components/PageFooter.vue';
	import PageJumbotron from './components/PageJumbotron.vue';

  	export default {
		data() {
		 return { 
		  }
	   },
	   components:{
	  		PageHeader,
			PageJumbotron,
			PageMain_1,
			PageMain_2,
			PageMain_3,
			PageMain_4,
			PageMain_5,
			PageFooter,
		},
	 }
</script>

<template>

	<div>
		<!-- header -->
		<section>
			<PageHeader />
			<PageJumbotron />
		</section>

		<!-- main -->
		<section>
			<PageMain_1 />
			<PageMain_2 />
			<PageMain_3 />
			<PageMain_4 />
			<PageMain_5 />
		</section>

		<!-- footer -->
		<section>
			<PageFooter />
		</section>

	</div>

</template>

<style lang="scss">

  @use 'assets/scss/main.scss' as *;
  @import 'bootstrap/scss/bootstrap';

</style>
