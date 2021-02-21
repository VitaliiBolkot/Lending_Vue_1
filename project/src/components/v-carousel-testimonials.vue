<template>
	<div class="wrapper">
		<div class="v-carousel-testimonials"
		v-bind:style="{'margin-left':'-' + (100 * currentSlideIndex)+'%'}"
		>
			<v-carousel-testimonials-item
			v-for="item in carousel_data"
			v-bind:key="item.id"
			v-bind:item_data="item"
			/>
		</div>
		<div class="div-ul">
			<button class="btn-bullet" 
			v-for="i in carousel_data"
			:key="i.id"
			:class="{active:currentSlideIndex==(i.id-1)}"
			>
		</button>
		</div>
	</div>
</template>

<script>
	import vCarouselTestimonialsItem from '@/components/v-carousel-testimonials-item'
	export default{
		name:"v-carousel-testimonials",
		components:{
			vCarouselTestimonialsItem
		},
		props:{
			carousel_data:{
				type: Array,
				default: ()=>[]
			},
			interval:{
				type:Number,
				default:0
			}
		},
		data(){
			return {
				currentSlideIndex:0,
				isActive:true
			}
		},
		methods:{
			prevSlide(){
				if(this.currentSlideIndex>0)
					this.currentSlideIndex--
				else
					this.currentSlideIndex=this.carousel_data.length-1
			},
			nextSlide(){
				if(this.currentSlideIndex>=this.carousel_data.length-1)
					this.currentSlideIndex=0
				else
					this.currentSlideIndex++
			}
		},
		mounted(){
			if(this.interval>0){
				let vm=this
				setInterval(function(){
					vm.nextSlide()
				},vm.interval)
			}
		}
	}
</script>

<style scoped lang="scss">
@import "@/styles/_variables.scss";
.btn-bullet{
	border:1px solid $color-border;
	width:10px;
	height:10px;
	margin-right:5px;
	margin-left:5px;
	background:none;
	padding:0px;
}
.div-ul{
	display:flex;
	flex-direction:row;
	justify-content:center;
	margin-top:2rem;
	margin-bottom:5rem;
}
.btn-bullet.active{
	background-color:$color-hr-btn-border;
	border:0px;
}
.wrapper{
	max-width:500px;
	margin: 0 auto;
	overflow:hidden;
}
.v-carousel-testimonials{
	display:flex;
	flex-direction:row;
	transition:all ease .5s;
}
</style>