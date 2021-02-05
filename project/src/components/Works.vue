<template>
	<div class="main-div">
		<div class="center header">
			<h2 >WORKS</h2>
			<strong>Lorem ipsum dolor sit, amet consectetur adipisicing, elit.</strong>
		</div>
		<div class="flex-center">
		 <v-carousel 
		 v-bind:carousel_data="sliderItems"
		 />
</div>
		</div>
	
</template>

<script>
	import vCarousel from '@/components/v-carousel'
	export default{
		data(){
			return{
				sliderItems:[
				{
					id:1,
					name:"img1",
				
					
				},

				{
					id:2,
				 	name:"img2",
				 	
				 			},
				
				]
			}
		},
		components: {
  		vCarousel
  		}
  
  	
  	
  
  
	}
</script>

<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Open+Sans:wght@600&display=swap');
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
		border:1px solid black;
		padding:10px;
	}
	.main-div{
		display:flex;
		flex-direction:column;
		background-color:#1b1a18;
	}
	h2{
		margin-top:6rem;
		margin-bottom:0;
		font-family: 'Bebas Neue', cursive;
		
	}
	.header{
		color:white;
		margin-bottom: 4rem;
	}
	strong{
		font-family: 'Open Sans', sans-serif;
	}
	.indicator-item{
		border-radius:0;
	}
	
</style>