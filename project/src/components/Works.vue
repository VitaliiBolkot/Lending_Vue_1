<template>
	<div class="main-div">
		<div class="center header">
			<h2 >WORKS</h2>
			<strong>Lorem ipsum dolor sit, amet consectetur adipisicing, elit.</strong>
		</div>
		<div class="flex-center">
			<v-carousel v-bind:carousel_data="sliderItems" />
		</div>
	</div>
</template>

<script>
	import vCarousel from '@/components/v-carousel'
	export default{
		data(){
			return{
				sliderItems:
				[
				{	id:1,	name:"img1"},
				{	id:2,	name:"img2"},
				]
			}
		},
		components: {
			vCarousel
		}
	}
</script>

<style scoped lang="scss">
@import "@/styles/_variables.scss";
.carousel-item{
	height:auto;
}
a{
	width:auto;
	height:auto;
}
.flex-center{
	display:flex;
	flex-direction:row;
	justify-content:center;
}
.border-img{
	border:1px solid $color-black-border;
	padding:10px;
}
.main-div{
	display:flex;
	flex-direction:column;
	background-color:$bg-color;
}
h2{
	margin-top:6rem;
	margin-bottom:0;
	font-family: $font-family-bebas;

}
.header{
	color:$first-text-color;
	margin-bottom: 4rem;
}
strong{
	font-family: $font-family-opensans;
}
.indicator-item{
	border-radius:0;
}
</style>