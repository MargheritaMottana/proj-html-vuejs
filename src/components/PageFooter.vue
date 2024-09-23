<script >

	import PageFooter_Top from './PageFooter_Sections/PageFooter_Top.vue';
	import PageFooter_Bottom from './PageFooter_Sections/PageFooter_Bottom.vue';

  export default {
	    data() {
	     return { 
	      }
	   },
	   components:{
		PageFooter_Top,
		PageFooter_Bottom,
	   }
	}
</script>

<template>

    <div>
		<PageFooter_Top/>
		<PageFooter_Bottom/>
    </div>
    
</template>