<template>
	<div class="testimonials">
		<h2>TESTIMONIALS</h2>
		<strong>Lorem ipsum dolor sit, amet consectetur adipisicing, elit.</strong>
		 <v-carousel-testimonials 
		 v-bind:carousel_data="sliderItems"
		 v-bind:interval="3000"
		 />
		 <hr>
	</div>
</template>


<script>
	import vCarouselTestimonials from '@/components/v-carousel-testimonials'
	export default{
	data(){
			return{
				sliderItems:[
				{
					id:1,
					name:"img1",
					textTestimonials:"Lorem ipsum dolor sit, amet consectetur adipisicing, elit.",
					fullName:"NELLY ATANASOFF",
					srcimg:'testimonals-img.png',
					job:"CFO at Atanasoff LLC"
					
				},

				{
					id:2,
				 	name:"img2",
				 	textTestimonials:"Lorem ipsum dolor sit, amet consectetur adipisicing, elit.",
				    fullName:"NELLY ATANASOFF",
				    srcimg:'testimonals-img.png',
				    job:"CFO at Atanasoff LLC"
				},

	 			{
					id:3,
				 	name:"img3",
				 	textTestimonials:"Lorem ipsum dolor sit, amet consectetur adipisicing, elit.",
         			 fullName:"NELLY ATANASOFF",
         			 srcimg:'testimonals-img.png',
         			 job:"CFO at Atanasoff LLC"
				 },

				 {
					id:4,
				 	name:"img4",
				 	textTestimonials:"Lorem ipsum dolor sit, amet consectetur adipisicing, elit.",
					 fullName:"NELLY ATANASOFF",
					 srcimg:'testimonals-img.png',
					 job:"CFO at Atanasoff LLC"
				 },

				 {
					id:5,
				 	name:"img5",
				 	textTestimonials:"Lorem ipsum dolor sit, amet consectetur adipisicing, elit.",
					 fullName:"NELLY ATANASOFF",
					srcimg:'testimonals-img.png',
					job:"CFO at Atanasoff LLC"
				 },
				
				]
			}
		},
		components: {
  		vCarouselTestimonials
  		}
	}
</script>


<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Open+Sans:wght@600&display=swap');
hr{
	border: none;
    width: 15%;
    height: 1px;
    background-color: #cccccc;
    margin-bottom: 5rem;
}
strong{
		font-family: 'Open Sans', sans-serif;
		font-weight:600;
		margin-bottom:5rem;
	}
h2{
		
		margin-top:5rem;
		
		font-family: 'Bebas Neue';
	}	
	.testimonials{
		display:flex;
		flex-direction:column;
		justify-content:center;
		align-items:center;
	}
</style>