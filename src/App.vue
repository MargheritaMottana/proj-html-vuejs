<script >
	import PageHeader from './components/PageHeader.vue';
	import PageMain from './components/PageMain.vue';
	import PageFooter from './components/PageFooter.vue';

  	export default {
		data() {
		 return { 
		   message: 'Hello from App'
		  }
	   },
	   components:{
	  		PageHeader,
			PageMain,
			PageFooter,
		},
	 }
</script>

<template>

	<!-- app -->
	<div>
		<p class="text-primary">
			{{ message }}
		</p>
	</div>

	<!-- header -->
	<section>
		<PageHeader />
	</section>

	<!-- main -->
	<section>
		<PageMain />
	</section>

	<!-- footer -->
	<section>
		<PageFooter />
	</section>

</template>

<style lang="scss">

  @use 'assets/scss/main.scss' as *;
  @import 'bootstrap/scss/bootstrap';

</style>
