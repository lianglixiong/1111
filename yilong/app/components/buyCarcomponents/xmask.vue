<template>
	<div class="advanced-mask-layer animate bouncelnUP" @click="closeMask()"></div>
</template>

<script>
export default{
	methods:{
		closeMask(){
			this.$store.state.isShowMask = false;
			$('.advanced-mask-layer').css('display','none');
			$('.slide-selector').removeClass('plugin-show');
			$('.slide-selector').removeClass('selector-active');
			$('.sure').removeClass('plugin-show');
			$('.fix').css('display','none');
		},
		
	}
}
</script>
 
<style>
	.advanced-mask-layer{
		display: none;
	}
</style>