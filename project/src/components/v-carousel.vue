<template>
	<div class="wrapper">
		<div class="v-carousel"
		v-bind:style="{'margin-left':'-' + (100 * currentSlideIndex)+'%'}"
		>
		<v-carousel-item 
		v-for="item in carousel_data"
		v-bind:key="item.id"
		v-bind:item-data="item"
		/>
	</div>
	<div class="btn-div">
		<button class="button" v-on:click="prevSlide">&#60;</button>
		<button class="button" v-on:click="nextSlide">&#62;</button>
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
	import vCarouselItem from '@/components/v-carousel-item'
	export default{
		name:"v-carousel",
		components:{
			vCarouselItem
		},
		props:{
			carousel_data:{
				type: Array,
				default: ()=>[]
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
		}
	}
</script>

<style scoped lang="scss">
@import "@/styles/_variables.scss";
.btn-bullet{
	border:1px solid $first-text-color;
	width:10px;
	height:10px;
	margin-right:2px;
	margin-left:2px;
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
.btn-div{
	display:flex;
	flex-direction:row;
	justify-content:center;
	margin-top:6rem;
}
.button{
	background:none;
	border: 1px solid $first-text-color;
	color:$color-hr-btn-border;
	padding: 10px 20px 15px 20px;
	font-weight: 600;
	font-size: x-large;
	margin-right:1rem;
	margin-left:1rem;
}
.wrapper{
	max-width:1270px;
	margin: 0 auto;
	overflow:hidden;
}
.v-carousel{
	display:flex;
	flex-direction:row;
	transition:all ease .5s;
}
</style>