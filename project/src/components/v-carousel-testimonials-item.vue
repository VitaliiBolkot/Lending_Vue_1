<template>
	<div class="v-carousel-testimonials-item">
		<div class="main-div">
			<div class="datas">
				<div class="div-img">
					<img :src=" require('../assets/'+item_data.srcimg ) " alt="">
				</div>
				<span>{{item_data.textTestimonials}}</span>
				<p>&minus;<strong>{{item_data.fullName}}</strong>  <small>/ {{item_data.job}}</small></p>
			</div>
		</div>
	</div>
</template>

<script>
	export default{
		name:"v-carousel-testimonials-item",
		props:{
			item_data:{
				type:Object,
				default:()=>{},
			}
		}
	}
</script>

<style scoped lang="scss">
@import "@/styles/_variables.scss";
strong{
	font-weight:700;
	font-family: $font-family-opensans;
}
small{
	color:$color-small-text;
}
.datas{
	display:flex;
	flex-direction:column;
	justify-content:center;
	align-items:center;
	width:500px;
}
.v-carousel-testimonials-item{
	display:flex;
	flex-direction:column;
	justify-content:space-around;
}
.main-div{
	display:flex;
	flex-direction:row;
	justify-content:center;
	align-item:center;
}
.div-img{
	border:1px solid $color-small-text;
	margin-bottom:2rem;
	display:flex;
	justify-content:center;
}
span{
	text-align:center;
	font-family: $font-family-opensans;
	font-style:italic;
}
img{
	padding: 10px;
}
</style>