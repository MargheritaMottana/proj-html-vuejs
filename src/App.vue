<script >
	import PageHeader from './components/PageHeader.vue';
	import PageMain from './components/PageMain.vue';
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
			PageMain,
			PageFooter,
		},
	 }
</script>

<template>

	<div class="container">
		<!-- header -->
		<section>
			<PageHeader />
			<PageJumbotron />
		</section>

		<!-- main -->
		<section>
			<PageMain />
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
